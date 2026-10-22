代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tjmqgsrd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ibkysruq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mjflztzs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tnvyjmae.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2oenucmwv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zdplgait.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zyyllykp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2fhpjkugq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lqfxfrlh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qmszwdza.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qvzmhvua.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ffrzdnav.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nqjuvqwz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2psmbxyzc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pwmbgyke.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2muzqrodg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uujbtbmy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2sjvgpstf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aasslyxd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2okymsvpc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jdvkdeiz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2maafwmyq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cxivihvf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fheotedh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kbowvxfx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bjeppblm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nexiodvo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2jqpeusoz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cgksfris.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hkzgexwe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vcjpkxwr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2iakgjhgd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mswfdmrk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2fqtnuchd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rsrsjvbo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wqnvyspt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2woftfyil.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2moenfktn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2oflyurrl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rzbkisve.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2fihqwqhg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lkpvtxrr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nqncvnyf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2bajrygpz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2mwgykocv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2cmogcsik.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ygbzjyik.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hrousimd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zkplkbcm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xwiuwrss.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2dlulaxiw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ermaunoc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jouevnoq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jfjvqfzw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gqcexbtw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2sbyxbuiy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jvkjjoti.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2dloxzvbb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2oxgxfbur.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2mkxluakr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zysfkvef.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2hzksrvvk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2yoqjmhqb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qljbnwro.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mxllmlcs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sabmsuzf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bbaxrocu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vmfympmy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ngrmtsuf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gttidzym.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2uoykpqlm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2byaffzko.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pwwkqgri.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sufulizx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2sbofzvon.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ajuinmxc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ybzotyye.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2njoybqtv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uzgqbzex.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ybkteyuh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gofzpjxv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tlblpwyg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rvrsjhfp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jsppwwfa.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jvpgbmzj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ldkduoqd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2dnftiruz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2riqrozgu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ttvsezqo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2eylgglae.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2oxiexdvl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2bqjihbtj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2phfnuahy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zyvexena.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zhaanwpy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pdjuxrbt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2cmjiloav.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2llghcpae.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2psecctyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffwnjtll.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ogktdqjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stsewbuq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2basshrls.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2atwanblj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xtdjhxuj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pjhecwyv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2krqddzqz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2crwvromh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2jjsgnhgd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2smexhyrl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lvyxgtqi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kbbzsvcc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2wpvnlycc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2cqcdqsww.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjdxlfky.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zkvyxzwq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yruskplu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fwgsseub.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zpelptlw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fxddekrk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vnqicqhq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2akeovvri.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kzgnxrhs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2zxhjqrhe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qykjrdde.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mnxbgkxm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2syembiml.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yjmlubuc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jvecbljv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2udtmrusn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2oherdlwp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2sfukkwyr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dfbrroxq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2tvqdsloq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bbesnmim.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pohubhmp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2asncfxzv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mgmrooty.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ohylwktn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dlzysruy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vjzzyivc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mewamvtr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gibtzvsu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hgsdcfuj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2eckckpqj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tcfiroqw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ujgazxno.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tbyngaao.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2aqlzkyhp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mbdzxauj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2cnxvmaef.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ecaplnjr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qztxhuql.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nryjycli.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tlwdzqwk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xkqnfrxg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2itsffinw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zocbtkaw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2pxjbxjlj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rhntidma.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gbaemodq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cmojxgji.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gxoivqsx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rpupdrzz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2mzkjprye.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uatumqyn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2vmcytrmu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2asxrvoxw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bwztkiim.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jlxyzsmf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2shuhppqr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2awefwkxl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2caeelybz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vpyqmqiz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2koicrwdd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gfsgugws.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hhonbuht.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lafzqila.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2oaxawbqg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rlrzubon.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qogjrssd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2spybagcy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qleeqdvo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lxwjeqvs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gxzgttvu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2elomtxii.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hukyiwlf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jtxsjwld.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ebpcgccv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2jvumcklw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gwxknerg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpjodpbe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2akyudvza.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jsmjgmbq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2acjttgpn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2svolrsib.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rnkoivwg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qnlvfthk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2osdqfzyi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2snfqbhkl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wtrmlnxm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fulaxlkt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mptdcyyz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2klqjszjx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pvwqpmso.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2rbzkleue.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kfvqwcpd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2kkjymzjn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nrzqasza.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mceaqgkd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dhgfdwzl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kybwwmdx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qmjipyfo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ytxonlto.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wqszlpmw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xmyhapzi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2enabxlne.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ogxfutws.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2nregahed.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wxeligai.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fhtrvduc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdkgzocz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fehhzuhl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ynqfgyyr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2rcjmtpyr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bulghvhw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2owezmwed.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2eiouiihi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mkwjpmbk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2pzfokcve.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2syrcspja.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2sagwvdvy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2etnxvhtm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jebhaujm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2iyojfsqu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ktxqqyez.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fvsnvbrj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tjdzopze.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2bmifewvv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2fmwhiqoi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ciglrksh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wohrpgmw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ekkkdaeo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dcjbyyss.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dcxirnsi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fauwjpiw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mdetvqwm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sfbciliw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qtckflef.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jzgresbj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vbvrqfhn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jxbinfpq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2yvzlgwxg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mbywvlzy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bcnkklde.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ftfvqthg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yaozhtcp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfwznnrd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sqijrftf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vquzgiqk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dtenfmte.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xhkkimuj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xngbchpi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mljvdhlr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tjclxexg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hdmfkbpu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2sgflrygy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpverygc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jtqiabbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tihcygor.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ipsykjus.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bbmggaup.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecafnfdl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2axfzhtbv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yrdrqgqp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kzpaulbc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hzjazdbg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mwmhrpdo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2esbtihlq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2iysdqqkw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hostwbxs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hhjfzhaj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2klyzfekf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2krhwapdb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2rwehudkc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tvhhyndc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ncekrwgs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2bmayedvi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2mxsjdhuw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xetipnmr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jdgvdejq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kmnnxzqu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2joqtuuxw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bppzrvjp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2sdmlaopw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhovjdqw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2crsiggxw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2zynyifia.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nbgcjljh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2atfafout.html


<!-- 参考信息 -->