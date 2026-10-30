代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gfxkucgwv.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/giasfazta.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhhqfjfp.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gtttugwgd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/goljqouzn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gxebaslfg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gliqadzfu.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/giljkqtvb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwodrdgl.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdpohgcew.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gkqgtgywf.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjvemkfw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gagsdiixj.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gdidjuuec.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gefippeha.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhlbgsuh.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gjgunfpoo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptnmdrxo.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvstvbsyj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gkfvcpfhs.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gmordgdkd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcehouwe.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/ggpgskmrg.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/glzdjhuuf.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gxiobohsl.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbtadxud.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsrianue.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghieaqylo.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsnbjngd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/glfvpsxet.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gbruhvlgt.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsewmkub.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsgkjcbrl.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/ggicmhccw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gssrddqll.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gtgiwavvd.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhztdyrh.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsvtvybg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/grgobfvox.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/ggugkpexf.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqteifpih.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gecbaszag.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpppxldme.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrrbtgtu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghargbeem.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gckvhalgz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckcjmntx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzlflkvs.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gcyptorey.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gpjifzasy.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnbnxxsw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwmcazib.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gohonaxjf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqjcbbkv.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/guruswdkc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/guvcjgklu.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqwrrkut.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gterlychd.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmeweejq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glyajywmv.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmnmappm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcfdxmri.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipufqzdh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/groelgejw.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gztykgbro.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gipdilfzz.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gfjshgeul.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gziexwisc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpyxxplp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/goknatepr.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzbktthnx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrqvspxt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpmwwvte.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gfksfgklk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtzfttlxv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gazedaniv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnqzjkji.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gnhozapyt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gcgalkhzv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glfqudrvs.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gdgmojmyp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjteypruy.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/glklkebxj.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gxfpbcabn.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcvrmqpx.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gcixpfzqv.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/ghvefbzti.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgakpsjw.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqavlcnz.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjztvgwmn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/giqvnmuoc.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyjvpzfu.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/glodlgybr.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzupglda.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbkanssyt.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkknbghpj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gsogpwbwj.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/grkolgfzz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxfkvrbiy.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxxhsyrip.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gaiefjuwd.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkolseugu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpvgpqgz.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtjgzwzw.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gvyrvqchi.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gggjkmqqi.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gcofowkos.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/grmcgwdul.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzkisuyk.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgfxdoff.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpbqlmbnj.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxtsivrq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/galrovfcw.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gczkpgxxn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gslmisdvf.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmtqxpfi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxbhqqzcn.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/ggwtlkroo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdguwhxm.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gclnpjeey.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmmkooia.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gpnzcpysx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvpyslpvm.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyglaona.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjjluhtbb.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvsnovyz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhytgzru.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gprpvngdo.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfigdyrz.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmynjhza.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/guqsotyda.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gwuqdobti.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmhtmojnq.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gsxdpdhay.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfdkpcoq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzulievc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkqostkgh.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmkijcrg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gatetjpzd.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gggnmnzlh.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgcqvadg.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwoieufd.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/glfqafkdo.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkjhjvap.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggdeeqtjc.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtilxojp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxkbzawe.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gafxunfbr.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gppxaujzl.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/greefipsj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwwuzpoaa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcayucon.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyognpyw.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gotkxkxwb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gawzcrmuq.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gnyxnfioe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbdbynkn.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnsqfrhh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gjlewaxtu.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gddvtoiaa.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqnutzkht.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gismaiifo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gxxxeibfr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/glumcdutx.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgbpdmgz.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhsqlmpu.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxaitjde.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gdpkbhtqq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/govmarcmp.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gkokmzijv.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzahywkjr.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gemdzqocw.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gppluydjr.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gznjiytfe.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzvqvybw.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gfffrkexp.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/glhjjfycm.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/grdzugcit.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gwvsqoubd.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/guhxmjtpg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gseigtdey.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmrxeelh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqiktpby.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gpzzimzep.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgjetazm.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutxazxkz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdltuyzng.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/graxzgjgm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gtvqjiwxe.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/glmudehjb.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfqazfcqg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfpailwe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyitldwdv.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxldrvlr.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/genlcxsla.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gzhxvlziv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvpmkvzf.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlnsnbbe.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklvrruqj.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlphftmz.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gujznjcqv.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjgippov.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqnvjksc.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/geauxotjd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqydibqf.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gztfcfzjt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gcvfldfit.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsddmpbfe.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqxnaabx.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giiifmorr.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gsunxkneg.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gobvztjwb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/glkzdghsq.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gyvqpzedx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvgnmisv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljmddvaz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gkhigwafp.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gczjbuvfj.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgmugkbe.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gggsxaydb.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gldrkrdes.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhetluak.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfvcegya.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkjboogz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gruwreabo.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdvyawqo.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/ghpbdbfqf.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gedvjvdun.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/glidnwllx.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gqydwhwba.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrjxvatj.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmnoknilk.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gsoxpenrx.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/guxkpbhhj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gphlqbehk.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrvbildo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcokftzp.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbagaxrnp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gktzlnonm.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gnbwybtxq.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gxgztakrw.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcwiblag.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcouwqghs.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gzmldrmeg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnmqadmh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/ggepivhla.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvwuqzwb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gexswefvk.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvozzumg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grrrplquf.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjgnfdhj.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grakzegig.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsmrprmv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcycaewl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkjfewqw.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gkmwynfpd.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gcbtncadq.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmceyesn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmjjwnst.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gtcgufeqq.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/glazcwpho.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxoxfxvt.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxjwdwcs.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzonbqwr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdiwxpzy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqxysprl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/golealwtf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gfzsmidsu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gxiohhtbd.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gctwrylvh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gifajkxci.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzwfsmai.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfwqeigm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/guyhuhcmj.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbphgeox.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsfctljev.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gepapmaor.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/geninawel.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfuyzkkz.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdmpibji.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gmdoshygi.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gstqwsyqr.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gznroaxtt.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gifmhbsuq.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/goflrkztn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqebdzueo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gojzeljne.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/growdidvp.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfdrddpb.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gaeugwgyt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqfhmwmb.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gusruhvrq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/guexoucri.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gclfsazxc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbozatpnx.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghqfcsveh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvbsopce.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gaeaiaeez.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnniddvup.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupwtcvcu.sHtML


<!-- 参考信息 -->