代发 wailian999

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gpmrwabxv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/ggoxoqako.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/geahcrlba.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/giaqfnstr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqrrbagi.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/guzdnoqxn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutdtjxzc.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhpatrft.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glnwqyvdo.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusvxwwsg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gwkxhohxs.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gbkotwuwc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gazgnhnov.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgxkblfm.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnlocpgz.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdebtnqlo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkruertv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/ggaoisqgi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gtujwlybc.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiysjwcz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gecmfujhy.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gelgdykkr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyovbbfa.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/ghktmnzwb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsjkiaqk.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/goniatqzo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gmrpvgyit.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gowlqtibs.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvorbvagn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohdhazvd.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/grthjplli.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwulysei.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghovbmolw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnmebabi.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyegpigc.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gdwtxaadg.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gtwwayllg.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywvvajrs.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gujdntzfu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcbwcjzw.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/guysrsisf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gtbjykkqn.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfmvnvdi.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/guepouuok.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grdvtoybj.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gevytshkp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlaehycz.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gggirsneh.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbqwatgcs.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvoepwvq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/guomlsnjj.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gtmlohhai.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhfeyejc.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gjflrqqvx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gupasbjub.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbrosswa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gudvabkya.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gxpatvwbf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiudeoma.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoamcqbz.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gdbgxpjzv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtqrvzkc.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gnsxkeugz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/grzednuuq.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgpctfxk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gvmxayboa.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/giiujiatf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gmqdtrvwa.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzqcjugx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqazlvrx.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqyyxanl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbicszyfy.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gncuuxstq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulhwligs.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrzaghnh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbakpkab.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gmzfptqpb.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/goormpuoi.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcciqdqb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gipxhfqgd.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gjgbeohrv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpqawnpz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzzddeokk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtacxjxo.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gvdrcipvf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gpsgqgfoy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxpoyolo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvraiixk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gejqcyioh.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/goxcvdsua.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoymtlci.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvlxkwpa.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gabhotdaq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gssefrpxc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnobefqf.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gbemzklji.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/ghashsdtf.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gafnigknj.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnaaehfd.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gaiflszey.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlxlucpt.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlqcppmk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gwuxwbzpn.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjycglio.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzbpnbnrb.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpanazck.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggstjbkih.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdypmwwy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxkrrgdf.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gkftqwizb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gdlezxpzl.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggywymakp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyfzgvnr.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpachsmrp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gumuwypre.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxumejmn.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gxshstkon.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gtjmrweny.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ghmmndjuo.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/glkznzbyc.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndgkolzz.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbwhwllb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyrhlenta.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbocynzlw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbakawxl.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmzmbutz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gornvfxry.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdomzfrqh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqtiqswm.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpavmuxgm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggabwozx.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/grhrskwqk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/grldabyyl.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gorzjcovq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/godsnziqr.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcptwslxj.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggofdmvqs.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfviwuxst.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glokuesrh.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmkfamhnn.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaijmpcy.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gopmzlfid.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/goqrxzzen.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gursoqbmp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsaicnhjm.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjwvezch.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcbuurlk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gctngnisx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrsicyay.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gacjstblz.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/grpmiaoeo.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklwgqnam.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gpszmqwto.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gemqkpwzf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjhlqvrg.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpgwslti.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/goekxcviy.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gyorlrrke.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlwpjurd.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaigjrnwi.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrylcwym.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiqsfgvm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/goezfexil.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guleymvzz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gwqfomdlh.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gtwsglsvz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbzmjqgz.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gmrbiclbj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/guuubwoqa.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuuunllc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdjoytpb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gesaitzki.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgzmzgjl.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gecxlfngo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegnsqxfy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjnmevqw.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbirewyc.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gjafnnpvp.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gxytthpxr.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/glwssncxq.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoogmogj.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/ghyhfabav.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggasqeetp.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwcnxsub.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzubmopa.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnssihns.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gppnfmiri.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfmihqyf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gbghowwvv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxdbnuxt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyjmtdey.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjrgclnr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvvrcgtf.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gblrtvgms.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxdrqbup.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfmzaisbp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoaaepir.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gswlogana.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxrmkokd.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnglxdog.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfjxpesp.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gpsgfidwu.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gphxgvwqu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyjchfdf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzmpxocr.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbqrrxab.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwffajfaz.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvewjdtvg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gfxfakxny.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcckftlfj.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gljkeojhm.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxndydklo.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gfiddenxd.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjuybedu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnivsjeze.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/glssgtsdc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghghhtnmu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowaiunyg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gbeacrvrb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynxndcwj.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gntfbkbxb.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsktxradx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqzokaux.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gnleekmtq.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/glbpfxzjn.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gzspvtjwc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcxcvrdy.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrhikkut.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqplipsq.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjnkyfso.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/ggxevdyuv.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfdnsmep.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gdjioaadh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejbajikr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvodsfsvg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscwurjub.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gejmjzkkn.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfnzorbr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthvawfuz.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gwhjqkate.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gtyqugjqu.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gojjcedbu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmfnzlzte.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/ggbevslxk.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gmodcfipa.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgdsfgal.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gawkbdpgn.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gybnhpgqv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/guxwbqlft.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnluwvnfe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcwfadvz.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gcmsuejdh.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gwladflix.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gslthmvha.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfotqtzuc.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsjrggji.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqvqlzll.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gamzkavnz.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gkirlltgo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwgvdsitx.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrdnapjh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guouibmzw.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnwifjbd.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/giabhcerv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guswchcxq.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmjnlwuv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gjlwkbkrj.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gxdgwfpmk.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gamtyjkru.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrhsfeuk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gkacckgrf.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdfqhmdn.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuvgwwcs.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/garrihjda.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gaefmbmpx.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gxzyziepn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/giylbgjsf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabjjuvck.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtqcuxzp.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeuchoeu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gpvfhsbki.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkhjolfo.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjdfpatb.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwfzqsxfx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gsunbijws.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvcpyaxs.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gxmghyiyt.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtcupmzac.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaxweubp.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gzjcbgkoz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girpkcbwq.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gpuecmrrb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gtthgpzjs.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywaymeye.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/glvffxsop.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxivmdix.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gmjyuukcj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfkxookwr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlwrrlkd.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gupamurtu.sHtML


<!-- 参考信息 -->