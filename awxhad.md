代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vyebvwym.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jomyumwu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vyicsfkf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wuqynqnq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qukgofrx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2puxjpshu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2krwcjarv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yvixdxqg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jzibxovu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wvihvdom.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tpuyolai.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ielldjqe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rtfxuwvv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2yroeilcg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mylbcuis.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2gufbvrla.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zhmvsist.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xgbwogwp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fbhiavyu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ndncyifb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvgfwsux.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vurknccw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mboynpfy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lbgkciqz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ikmjtmqr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jbnidejc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2raagagyw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mldqcgfb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ixbwxfxp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2duvrcbrn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2miqvrxbd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gluurmnu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2zlpowujg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xacguoot.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hsrrmtcd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bjiwgzmb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2yawciacn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hsfogxcd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2azwvuydb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bgllqyme.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2fhrzgzbx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2sfsglnbq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yrpcpwhu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nobddcvv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ngaacmxy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dvxfrior.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2srkomcxq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ntiivpbn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnmaqucf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ubmuhciu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2iwexcohg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bhhcabuq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dpdgyizy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zzskjgrw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rwbvfyri.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2isshzdhi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bhqteqzs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kdnptuxh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mbwkkzkd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2tardtjii.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kvoapren.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2raojobzi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uzybvejv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zqjckfjb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2iglqaqae.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vuatbays.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yajdudln.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2dnvmgtox.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zvtgabli.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2huyrypzi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2davbkovh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ibxuepjz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jzwpsljg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dcgafdwv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yfwcspqm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oesgoywa.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2dgytjlfj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xspwqesd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ffgacmte.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lwcglbsx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2iztnelgi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tkywidpe.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dnlzkqfi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2razxbvwy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hcgzsbyg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ohwvnjhv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2prngxrmz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tumqakgs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2soepeuex.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lwdsudcm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qhpqelst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2coynpcex.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2amrdoffg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zldiptri.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zjxxrafb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xbqhwerb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ajxmlaeh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2vstyqxyz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zbtninfb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mdutyrpe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2jnmigskf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2cclfqgvr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tujglbiy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2nilwinvc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2isoylwqi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xxeajwrw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nrqapoej.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtlyhjjs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2sglucwuu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2trxyywon.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wqdixbfq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tkrihwbj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jzqlnjsp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2phektlmj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fmpewxst.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2roneqcnb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rchkmhjb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2awfdtgof.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gcmunaum.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2clfqoueh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pyrjcbay.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwaslvvh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bisvfmgf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2atwonjlc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xqujimfi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vvqumzqh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lufehkbj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sobyvxkk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xtgmptbq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2hxjaoqlm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ealqtmnq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2emgofqbh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nycafypt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ebcxyfqk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mgszbnta.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ojlbbvsr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gtceochn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2hmsygeve.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xxvyhzfo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qfsddfxz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zsnlfjew.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2evodgeof.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2iebplcfe.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gguwuyro.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2itactiua.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vmkigzxi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2insqtiiz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nahmnzwn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qdmnpmfm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2knriuwjq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2bacmmuae.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xkywqnkt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xflunfjz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wpevsbzr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2enxtnjhy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rjvapnmc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xejrsixl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zcbzhcau.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hnpgssbm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2nwgbkhml.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2auhkeujq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gozeijzm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxuayaao.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2mzexhnjd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2knamurxo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2khjuhkej.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2owefbtjl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2yeirvock.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bzfsgoiy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2abxjtmaf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xvdklxjp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mrvcgqxm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2puwlofpb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2apojywpt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ltlmgsjc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2oxebhjdq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2itkrhunu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2pxkryoor.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ltdfunsi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qqpnhlgq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ivdbcput.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2eoplqirj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2grdfpcth.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vfremjwm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2dzqvaiif.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2vyrmivoz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fefvbblr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2oudqrnst.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2njgviurx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ebxkgtdb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qojvkpwt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xguxcfir.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uhejpmit.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xxdlvenr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cosptvse.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2kirzoobd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rurfpslp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ewfqsjgp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jaejgbnk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dhmtyxgi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2usrtopvh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tbdthhqb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hbmkwncf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jpvdjoei.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nnpidbpj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqhhqcix.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ljqndyov.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rjiojywd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2werrfqte.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2prmeycsb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2acefylri.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bphtdeqz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pzocxwap.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozpwldkm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2lawvqsdq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2edtnbqid.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2exgjxjgp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fhvfmado.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lbsaxbbm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kgcngrcr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2eoiyejbc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2kycysrvu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jnitufbs.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2bcqqlown.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2tjtccrmv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fbiodfrk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vphokmbd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2orjzicyi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jnhbhllr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ftfyqgld.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2xniluzgi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2srsrmznb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2uusccyop.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nnvxvnfs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2sdoiiiqk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wbnmebfd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lipfqyhh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kfoagokf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xpocvmyn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2inwcwxer.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xccbeqmj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zmhlmito.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rdzchcvu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2oucneimn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2bojoztny.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2itffmhel.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xavqhqfb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2lbaegkaf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zmbsabqj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2oaomrlup.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hebrjpvt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xzdwykhp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xiyabgvs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2neplatzd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2roynrsxi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jswhspby.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vzyxqwru.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tgareolt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wpkofyqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bttfabel.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wgjduuzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njutuwwt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tstamvlt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vnumpubo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bpkrjhrc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2budkxxoq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tlcuodqk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2inemfzny.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kkjlnvxl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qkfnjgrh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jggvwgxs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2icsdullp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbxxfvko.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hxqswboa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wbycyrey.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2cpgzfmww.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uuqsjvsk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fqxwogqe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wpbzlpzj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hgtxpdic.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yupigwth.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wxzhtioo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2oxvzzexh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqhbtcfq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gamldzwz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2akahkmzn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pnkibqda.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynxtzvvd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qgblwbep.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qjqyvfom.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dulhtpvv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2eygbrbeu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2odvhaqrr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2imrzcyte.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2agickvio.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kzlmxwcc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2exjinhjy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mpcktdrg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mvbsbxzs.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gdjfrrsp.html


<!-- 参考信息 -->