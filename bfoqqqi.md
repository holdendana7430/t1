代发 wailian999

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gjbgqrugl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gikjdwvyl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gkhnfggly.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwovvkven.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghawejqit.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcqrvzls.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gkniyjxbz.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbrdwtxo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqleznxv.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goidlpoet.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpckyxdhe.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwsbyybs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gglnrvyfu.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfhhypzf.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvhonwks.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbpbdspz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeeugenm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhbgsplr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gvefbyelx.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvevxnia.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gipmqhddz.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gwpsfesuj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gmkjzzntb.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/ghqvlurpr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gfawlvtvv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrubleeo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtobgncm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjwbzoihk.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gevuiwwml.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfutwhyc.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvhzxmtz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gnrpymrer.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gohnacqym.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrajbiea.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsarkjph.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrgmpuse.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhrdchxs.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gtcfzapgk.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexamkgmf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfpklmum.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaggsbumj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcmzzyio.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapiashwl.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gemxuqwbx.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gligoheuv.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/ggoquyoua.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gexqqvtqe.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/galukkbxp.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhkuunfy.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gdrmpdyjg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gxooqbpmc.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gxhhaiovg.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxpwaxxr.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gzekuvhzi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjxsedmp.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gncezhxsp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gremtbsiq.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gdxzmfxwk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndjakopw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzsibwnw.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkwidugf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqjoisls.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/ggvscrytv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrqrdygu.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdnoatdrv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzqzuyvr.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gtoylqcsm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gxlefnuyp.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gntboofzs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwazvnrzd.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrnwdwfo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glbyyqtbx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueqhdjav.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxxmjonl.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbrpzohbv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggqdjhmdt.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gttvfecho.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvljknis.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gwxtruvco.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gfbjsuksq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gosbeyvta.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/geiwzmgsw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnuergpz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/giwxppzvu.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gxalroyer.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/ghcgenrlp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuesvdkt.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwnsshiw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gjmmbqyzo.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/ggiejqynv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpbumxji.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcmklbjd.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/guzwrtzir.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gptyctbnx.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gjgzwxklu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqhbrhke.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/goyscnuot.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsirhohl.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbamnxlrd.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyxlygct.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdsemsjx.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gycceioud.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqqforeg.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gbozwvmce.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtrwmzmz.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmhtvtac.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbkghsfoy.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxbbctgl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giepetnkx.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gujfztgpc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gporrbxwk.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/glbqsmobx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gecakqapu.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/giuvtwsgn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gonyisvnb.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gykbftdgm.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnkquapx.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gauirdeut.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gresqkuuf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/geimdhvsx.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/grkozdksh.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geefxxouw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gilpbpsaf.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gexizzdmw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuadesml.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gsjfdppvk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggmslbyzl.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpmizlkw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgxytzfs.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gvnwlmoja.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjdocxci.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/geprtmxdl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjxxowct.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gcsvorjll.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gndnthypg.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtzbelwa.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkienaibs.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gxazafxvu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmwefeodu.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gdtyxyepy.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvxuzobu.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqrpnvkq.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtmlojwtp.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gntkaulmc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcfnaiin.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzasidrff.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxxdslpmq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/ggqvryuoz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqfkvgjmc.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkfhpfsf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gybhjalho.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gmypfcblv.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpkanpcc.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrkdcxud.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gciiuasin.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzxqtubmb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gysposdmb.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gbuhsvmpo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gwcykhmrb.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcuvfbfp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfqupxxm.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gkfzyllgg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvuhvimr.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhfomgah.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gwqfemyuo.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwcvsbfd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxfqfyqk.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/geddpwniw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlnhcdhu.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/giqqiiebm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiqhpuce.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkkgprfz.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gydswjixo.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gnxyshumr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gohaamcfh.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gulyfgofe.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/glxylfaoy.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gamrwjsxi.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghabxgvbp.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghjygusvn.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuzenrqb.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpahgljyj.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfualyvj.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvlcjclu.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwsthtjyb.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/glitbxhzs.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gkgwnxrax.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkhbwkzu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzybicyfv.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gfrwcmnoq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gvnuwazuw.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/grzwxggfn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjafjcfkq.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gssizqrpa.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdmwkhwl.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/geutkerkq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gklqavhxd.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gapucoyqz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbpxuldi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfugmsve.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gujnwqfty.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzqqvjsw.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guohcmulf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjdhokah.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gemaoaloe.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtxvbzcsf.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgzmwbmw.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gjdjvfinh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/grcumsjil.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/glpqsohpm.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/galvimhnd.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gamytcqij.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlhkuraa.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcbdkepjd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gpplxjskw.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gcleutdlg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaipkztt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/glblzyxsz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfdgivnl.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gfeeaalnb.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/guwvhioqx.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyjptfwep.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gvpxxwnxu.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/guzvqwtmu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gegwofhuw.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gdwalkzvj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjaphghy.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhdmdaai.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnqrepyz.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjhfsjfi.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gqteyfzcb.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gonnptwof.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gpvamoosc.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/grkljwrss.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glqpkqsti.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzhhaigu.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gwlekcopb.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gvmudkeix.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/ghejcbkdq.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gspcnsbww.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/ghawvgenk.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkrjsgxo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtccfzrtm.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwwpkiixv.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gewhtyyea.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gactywehx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/godtxgfwa.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/giadcwzas.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaixiqeaz.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gknkagtxw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/grkevdypr.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gngymbuqw.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gpuynbshn.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvjdkbcs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/glpyrowhi.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogdgitut.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/getbigxfr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfpizaph.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtbpebwz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgbzprhs.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/grgtyjaiq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxcrntbr.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdctmyyd.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gcqccnrht.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunaiehmi.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjqvsgxb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrtdgbwr.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpoediqt.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gcvxgxbma.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gmidcuhca.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcxlhnyg.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcozxbzpq.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbsouwtr.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsuxlqgsx.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gzekhqjho.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gtbbzghpl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmecuqjuo.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/goifmrrxa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdnpsheo.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmmoveck.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gebgjjbrd.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkueakzwt.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gglxwhdhl.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gubfnktip.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmpnchah.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfglgezgt.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcevrvon.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gznoffxti.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gdblnqoqi.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gmrbkmgju.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepsrrasn.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gfmchkncp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gfuqmnjst.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gaeyvewin.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gctoxsyje.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmyqcnkt.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/guhzapbiv.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/grrzvqcmh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gvcdqwfhu.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxxnwbdwq.sHtML


<!-- 参考信息 -->