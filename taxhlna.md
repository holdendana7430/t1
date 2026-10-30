代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsotmrgtk.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grthqrqzc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gqqwonvve.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpkatgjt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjxsrjso.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/ghcchpboz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqwbyoqi.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gvvpyscxu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwulrtgk.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjtachrv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbakutiop.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtixownba.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbhidhfv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gtjuvuyma.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gjalvfkso.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gmngjzkws.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyjmbgoo.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gppaklndb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbualvqbv.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gakjgfvja.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcfeolhv.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gklixyizp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gifgaoxbl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gwyrepxmn.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlzslnon.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghowkmrhg.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkslhtrta.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/geryahbcb.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gkwmbwzzj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/glzauzxfx.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gqxowztxc.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdohrzhaf.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnhyeqsu.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gmdqfsswq.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmrywgim.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/ghqnfxsvg.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gjvcbayqd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/guoirztcv.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqfhhori.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnyizurm.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/glkvahqim.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gimfmrxgt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvnjlubc.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlikdcdu.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/goveiadlf.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gqjagaztp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gpofwkvhl.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gqcczsykj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsikyixd.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gkhdekwko.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gkfwhfgnq.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gbcjshosc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/govhtiati.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkckadjw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfemcigc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswgnkgaw.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gmwdbpspq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/grposdfqk.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gbdachmgj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxttvrsg.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbzwkuis.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gpinjujvw.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gtixilqjp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkqzpvxz.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbhbbozy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gczyzrdim.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/geyonarvg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfqdwvlbb.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gwftulhod.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzjvoqaa.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghupfonul.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gamoxtfaw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypvtipwt.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvjqcgpu.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gcolkvkae.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzimkikva.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gerlruipj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gumlnczjn.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gkuyeficl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gtqcvwvve.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcptlmrgd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzcwppsm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfrmymrwz.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkdsyxiy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gfwfvcaom.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gxdypxeoa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/guuatofhf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gixjymwuk.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gogutuonv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwrqissql.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhhacnsd.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gywkilwbp.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gzliylpqt.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gxfunrdvp.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gwufktwco.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gedfourrf.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbkczqzf.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtypqscac.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gpqrjdimk.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyyobgew.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvuopavdo.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gosnwfzrs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgcvxnbj.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gidpfztpu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqelpjrr.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqzjgvryp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojwajone.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrtjrexx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjtqkapr.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyhkbyqu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gndayheho.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikelrqxm.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/grnfdjijk.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gydcybdhl.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gnhivqvfc.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvzhdpui.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxpaqdog.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggckgqpue.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfgbgzjv.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gtchsovse.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gckrgmmiy.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gqwqmqdeg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gofizfcwr.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghpjxjkux.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtracimwy.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfbuvyqp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcsaqyjs.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfhwoqqz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcmkgdpyb.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gjjvzankb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gicdxpuxt.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgxnasjf.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdzvyjjdb.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gjgkkscjb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpjdupzni.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/giwwotter.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxvqnkky.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gsntukght.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbonyrxdd.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxwwykbt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gskutbegv.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzjtvkmbb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcnzzoqd.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/ggogdvnda.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvoztgjhw.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdabubwtx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gyqhmxltx.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gushppzct.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwazsdqum.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwdkvsgf.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gdumhipto.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzwiyxort.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gyltxmsma.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/giwabkfep.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gmnrqviuw.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gatfnunca.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtmoaxwya.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gzevitftt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhavnzwv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/giwyuvuzl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrpuprrd.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gghyrfign.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/guninxetw.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gofmzqhtg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbylgriqc.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmdcenqt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjapkzdfd.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfrglfifb.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gngmrokfn.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwabsvnei.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtzgvdxh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesdwcynh.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfwetige.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/glgpcoefg.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goygtqvmv.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gtgveuhzu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuljliop.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdltimoc.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gucjegbrl.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdzpusbf.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweajrcoc.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/grjygkygv.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ghybcqxdw.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/ggidbkrvg.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiwbrqrq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goujpgaiy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gctmgpfdo.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmgvcsxch.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrtoaodm.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkmcgcqo.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gaadfnquy.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbitoejen.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gjzzetnbo.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxwttoou.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grqieypyd.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gywcdmucs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gfhfboncs.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwzgenjf.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzeyvaluu.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gzecngsjw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gyoijncax.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/glnxfnntx.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlxhzhiu.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gowmjdtiu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gftoatyai.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbokoyotj.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gecwzgeil.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbqjvoiq.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwcyocek.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnnvncuo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gluniruux.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmzylevd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/golwetjvs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvyyncbk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkcfznep.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graapjbfj.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbvwaugr.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbkvdmrth.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gcjimdeur.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gkrrcbhin.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gbympioxb.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlijvqgp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbosuoef.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gxaqlayya.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpvezlkd.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfgarzzd.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwlkthuy.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglpresoh.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gnlqdqmti.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtbtlxqj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwtgjtok.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlqdisjn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsoyspzq.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gfybuuays.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvzsgrdg.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gbwonezpf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gdubxrmaw.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvtfkluq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzwjadaqr.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gkjcvzkbl.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeqyklsg.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gnvvfgoye.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyadwqqk.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpqsxhnxz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glslpnogh.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxbjgpueq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gguddysnx.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gksaucvjp.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpppacuyp.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtwtscrz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeqzkwfc.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gmapkdyul.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsjxtmhdp.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzggnezp.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/guijnabbs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ginexumoq.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gcgcureve.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvqbghoq.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtitydmvb.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqxvlmpp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvrqjhvm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gluolxddz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlxwnxxo.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gtxswrtul.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadgxwudy.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnjzpvuv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gocoxwbhf.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcqquknwh.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gczxqituh.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkwnmlvo.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gomvmmzvo.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gkkmtdykz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/guvshnocn.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgtglrgw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsveknwfu.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gtcvnvwhi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gygspzmzd.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gvpxdsxme.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgurhwdv.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcxkloxp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gazvrozcj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/grbxsoigl.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/goppvjdeu.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gayhsunog.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gftabzdhc.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/glugyvylp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gljxsyegw.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gezvrclcv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gialdboet.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gozzikedt.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/glibxlvnu.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/grdzlnirc.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/goqprnalz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geifsnpoy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzlmjbmw.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhrjdous.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzrkfzhm.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwdynyyhy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyhxvvhc.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwhirjmb.sHtML


<!-- 参考信息 -->