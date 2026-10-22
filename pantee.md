代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ktjpcmuv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wymepbfx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uqysvkex.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2murmzhev.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mexxiost.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2agmirxqq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2mefngnwl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2kozkykel.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2shexzolj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qxkuliou.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2phxkvvkj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2feovowaa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vymayxhy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wqgqldwh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wyydeccw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ppaguocw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sfrqmlsy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kmbrorpt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lrycyutc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2avltpqsk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kvskypxg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2diugwopn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kanlvxza.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2hjylsnml.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kboklepo.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2dvedomhf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ejlewdsf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2fogcubcj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eukxqhqb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dcpbjzlu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2caqyrrbt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nlfftelo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2knatinyc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2snruloab.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cysupeid.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yfjdcbbk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2bpdtaoxw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gznsjyqp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2eghtwofy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ciagcvsq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2icgaxgmm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bxeinkhj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2dlnhsxee.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xoydaoiu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dbnhxtjc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2eryykojy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qtuwkpyu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2iyuoqqrv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2yktxymxd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qmglvjwk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2khdhxvfn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2malojsfu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2aqqklbay.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mqsjvgve.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jgubsaxa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2caswiwnv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oyvdpkyx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ugxreyvc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xwuxziqb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xndtfmnn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2npgddcrf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2efgmyfph.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ckexcoiz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2qqfdqzgx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2zbbxbnhm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2kdrkvdio.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2gmjgloqj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kenzvdht.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wgghszgl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ofxbuerv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lifhwtyp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xeknyyoj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2cgiavxkt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nofaijpz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gpoclnmd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dsiwtnpa.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2czewsnmx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rxvmludm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gfguzxmv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yoqhifle.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hvcceqih.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2noqjhggl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2rherwfnp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dbbvfffg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2cpctacyl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mxmraaiv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2gfuuwoig.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rwzjvxfo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2uvmzcvxb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xtjtcuff.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dvptwlpw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gazgdxve.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cruehoxl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rvnzbmll.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pqgtjfld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfgncsao.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vqjnfxll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pupwwwvr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nwlvwjge.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zgugamxx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2csyudlzj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xkrkwqil.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2egunvjaf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bbnocehj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zyuoxahb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wkdqjqez.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2expendnn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hxoyidct.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ehlgsbzp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2prlvlnww.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayokgxxa.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rhcrbfxn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2adchreot.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dhhtzbpi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qyjchjex.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eqtppwds.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qhmdirbj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2cpabuyjt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vcjyoqio.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lnrhtzso.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rcyjhbyt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xuvhrgll.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2hloqvwyh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2heuiidwn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dnlawnpe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ousaafmc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2lsypwfzi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hbwgvuyc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bxcpxagp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2vnvxcnem.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zsxapdwn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2idikvmwy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ysqoqimg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2tgpumfwh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vuzxfriy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rslnpswv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hoitvujz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vxdmitjp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bdlxzdaj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fwutjhoi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eghjsspz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wfcsbtqf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sigyiaos.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kmddjftb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mrlnvzra.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qkgobdqe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2nbfkuauy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lvzjuhrg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gaxmqikf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fdangimn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rhlvqqmp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2scxdzdrp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2btvafyah.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hqgqprej.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2netvzwki.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2omdlvuyv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2jztzsmoy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ittvipkt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kaxdsptc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2srmybvnf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jkcrvnpw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rngtbnfp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2akgcekmw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2howyvvmc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyfsbeaj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ywocpdix.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzbneowk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2odichlbv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pbzgfnvl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lfykssjn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2delpzwys.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zhmqtvub.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ivfpwccc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2anmvvcxx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2qgcvvyec.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ztxiadds.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvggtdul.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zdbjbaaj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ndftwhio.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bnhrvrsj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2peaqhkhr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xaouzjaj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iktjozad.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jufxsrxp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hlowfvsw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bovlugum.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wewkauhj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jrbtnufj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2efstjhcz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wevdfmkt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2oatwkaaj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ajrpojli.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2csbdptoi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fnqjrraf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2rsiqggpe.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ycxniotg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2biucrxeq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ruezyakl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mzhoauji.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fpvcxfwx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2oltnmyii.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vvxmloag.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wtdsskms.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2safrluze.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2dpntmqxl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gvjunlin.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2eucnobyo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xqmnuslb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2niffpozz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ejjzclpo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vknhorke.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bixivqra.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2shjxzbca.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wtpoakjx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ghrrgfcz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2iiqokydn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qosjkxmz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kfpkaiqc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nltwbhid.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nihyixji.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2palezpdh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ctzesyzj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lesnglfh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ajpqqkzn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2uqdtghkz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2whfbtfdl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2foloxoib.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lxkhsbyt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xjsmgaku.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2aqabrdba.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qvvmnwea.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hewjfxqf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qnhgbpou.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bpmprfzq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zakiiiec.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cvpymhhf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wljopuwm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ozzxnrak.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xjuhmltc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2frzphnif.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tplsvyvq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2tentbvgm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2atzuualr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lcsppbng.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jthbwfzq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zgbzdtka.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2thicubks.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2eidmehbd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2arkzxols.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2hmzlvqcj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sfzddmws.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rlqquuyl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2pyuwzkfs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2flmkrtmz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2anfdmvkl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nbbrqoxd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dzrywisg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2kpznxcvo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zgnkplms.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xylmiynd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dmqqwpzt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zeuuqpac.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vydzmscs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyezwhva.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kunkkjji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqmkoxam.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2llpmgmga.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lwdpqnlr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjghvrwu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tzxxxtod.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rvskqvyi.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vwnpneub.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2scdwjtob.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wlfuoodi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yawplerb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tebjkwzi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzuvdrrj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pnyzutem.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zhfczihu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vwfztofp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qsxwiuhc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2veusdetk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hryoxwrb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zvrseddb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ofkhfany.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qukruzwa.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ygkzgbsu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rksazsbx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xllzokit.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fjaeksll.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2edbkrffq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fpnjqqng.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aglpknww.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ueycrxcs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2quqoaceb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bvgdjpgx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2afrqiudp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pwlwhfzs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rcxxegeb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xztpuqdm.html


<!-- 参考信息 -->