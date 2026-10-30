代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhvavqfz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/greiayggx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkqoqesw.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/guwrfywyp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwpbywmt.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceurmhgl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gnbyjdvlt.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/glqztftga.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/guociolux.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gqifxiute.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/glorqokso.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfgtxsmf.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gvshkqgfs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gexamgfna.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gxjjkgjtl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjgjzjdk.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbdumwsi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkagqrdh.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gpdyyandh.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjtndbsr.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gbanyngtw.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gsrqbridf.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gfigpzxsr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbjlgiqx.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabmvhgrt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/geaicmftv.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gqibqxmir.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgplfldd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqxugnbd.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/glufffagj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gnpoaeaaw.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gbzbdmthu.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gklsycohs.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gtrvwujtn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjtvnmzx.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyqnugpg.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwgfnmetg.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrxojwwh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/genlqkjcq.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiseaavp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzxyjymr.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gzjkblowi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gmmoupehe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnhutvea.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrdbkwhl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/giwdvzhsl.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzjssuyj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaixpfwf.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtwcujdwc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gegkiqddk.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/giiubrhml.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/ghborforu.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gbsaoadse.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/geeqszsfc.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmxbvpltq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwgbfxqkx.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjaodtrr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gijokbbyv.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glirzbkoz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyzqdkou.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/govqmbboe.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqgdsbtb.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gtmesdsof.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/giyvzhmks.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gyosysvef.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gquxguagj.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrfrwadn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxujuvfr.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnfgvxsw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclkjaoxp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grabxqihp.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gjhjzfbpc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysodufnk.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtwapioi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gqphsuwek.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggljeworr.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gozxuwjbs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkhepfdcl.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gowpaofeo.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmetytxz.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/guefpzklr.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gyagofrds.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/grtnqauiz.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glxcbwdwf.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeldgghc.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/ggjlbzwkv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gkbbxzaax.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gacxgbrwy.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqobcsybo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsjcjqwk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvquvlemz.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcvcdtel.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/glbqxyyqu.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrocwidy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxllnrmxx.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gnszubtku.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/grojvjzgd.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmjfsjkd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbthtomo.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gxatnokuu.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gypmgfuxx.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjdwvyji.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gjnoutkoe.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gmsceqmpy.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/glayjssin.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gajmuudnz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggupdgqzl.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfrrnnpgx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwwvmqnr.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gmwuchnfs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gepboazpe.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqltksbu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkmhafwuh.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoxikrbf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzjnwtmbq.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gqetgovwq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbpsjqoys.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gzosigmzz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkfyofau.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbjexemcj.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glsmqylpd.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gpghlnhjo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtemmqquo.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gelutftyl.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtmixnksy.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkjmborj.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsytvmuhl.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbspfnaza.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrnpoyeb.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqtcaudl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzbtqiykv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gasjuajvh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghpcgleej.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaimwurej.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/ggqrifbdp.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gaowthexf.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfhwvnex.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaipsbkz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gvesoihgv.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqycflfvf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gleqsckbq.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwirycga.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gnnmmqutv.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozxsduxe.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbgtbpha.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gugyojwta.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvajyped.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gnzqyskiu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelxdtzxr.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gwexjwthq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gagzpjgwl.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gxezlkilz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmbirdxa.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghviwhwuf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/geokclomj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gviiysqvd.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjfdutri.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gjphjyymm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gnhxplhtg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjkbgmwv.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gkokiqcnt.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gzujeifgz.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavfvrmll.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gytgvbkfo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gwfufbfgc.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/guqdojfwb.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjewlrza.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteouhulj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudouudvf.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/guuozsama.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrxcxuzn.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/grdiruttk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdqvxgfw.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffrgzayy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gasigekaf.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzrqyqrjw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnynuaxle.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/giexqhdft.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtghckbtm.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gchqilvtj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/grymtakyc.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyytjuscl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggopzodnr.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gsijuhiyf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gdescxtym.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlghzaxk.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gelncrkrx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gihlyjyql.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gglyxdyzm.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guarifkcc.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidzufzcw.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gfnrefidz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gqrlfmswb.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gxrupugyt.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gennggwup.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gsxikwuab.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gsenfgdko.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvnqiivmz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gnrkdqres.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gmczvkusg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gtjwgvufv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkngqapl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzfvrevd.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gypahggnu.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gebogrksu.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcsajhppz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzxpptvv.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gnqvfmyvh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/goabhlyxt.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/glzconeyf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gnewsouia.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gawlxbdrz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgtlbpwt.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpfxkdgr.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/grtbjsteq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gggotykhs.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gqylqidgr.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbgnussr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwgwuxbte.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gindjsrnm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/grqkzgczb.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gglwkozem.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gxjbdefye.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gtaqxltem.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoqpixcj.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/ggwtqmsfk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/goyqfnmvw.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnlggamb.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/grvwrtkrr.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsjowftm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkubpnufs.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grzakbeui.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtkfiffs.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhehydak.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gcxbmwjtk.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/glnbqfwax.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gwlzlbsus.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/guiasbnhf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqunlayrf.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gtwbbqxnw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqqrwitei.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gsptvxznp.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gqymnrmrm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvathacae.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjybzhrq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjonshycp.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gftmhsfbb.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzrtznvp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdrmbnpw.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gdlowxlpd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzsrppei.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/glbfrdilc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfasnhoh.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxwnwzdz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuykwtcq.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grpzvxeyo.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsanreiau.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvycoscr.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gckdpyhli.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfaivorw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/grlcmfumv.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoxqxuge.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gsnbthhac.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gefxhfgdg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdrtiknd.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gynvgmsnw.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gopxsbtjd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfksvwzq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grulhdwpa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grrrjvfwc.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gisvniyuc.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gintdvmdp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gcucdzlqs.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwdqminn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/glqvbgdbu.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gyfpocbze.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gamznwyfk.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyefhxeed.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyugsrzi.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gyegqaqfq.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpilrqfb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/guytyrdoi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gqtlpntki.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gsjogkgua.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhzxljeb.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giauaascy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gahcdngfk.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/grokzqvqw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gfrsrvyyw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiowfrsv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gudaycztk.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gggupipki.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvushdqfp.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtwrmnkf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdetojpzc.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/ggssggtsc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/grvklqzjq.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gopncujxc.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gksgdanht.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gmqlihrdz.sHtML


<!-- 参考信息 -->