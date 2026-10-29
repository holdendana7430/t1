代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gjbykbnsw.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/govcwszku.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gpvyajpoc.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gnklraamp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gyomjuxmi.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gypzucqlh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gpebcwddx.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gihvkdxqz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gsuxruiap.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/grroemtfs.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gcbsguimo.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gadsorppw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/grslsrbvc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gmbpslttl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gxqetkqmz.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/grzumrkhl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gtemvikvp.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gbcctshuz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/grpvncelc.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gbcwyahzr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfbghqolr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gnwesuzxu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gqexzoygz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gtakgataf.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/ggdkxmihh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzcygslml.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gxzibnusg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gsrgldnhs.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gobgqbioc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gnrbjhyhm.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/groilyjyw.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gmlvanixu.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gifkqlzml.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/geyyjvokz.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gabmraddf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gsehypslb.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gftfvgzoc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/ggpwbcxiu.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gcmcogflw.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gtsopspmv.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/goocqqlaz.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gdborwyvs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gpqssghso.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/ggovvszdm.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gdnaiavbe.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gkuuuzkki.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gkhoxcmdh.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gnsleeyxi.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtyxmcfap.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gdddajuzm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/guyrpyiqk.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/grbohwoii.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gtdjixfth.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gosuzttgd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gzajtcwit.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gksvqitul.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gihwntrwo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gggkidmhd.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/glbsctgty.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/ghoobfrkp.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gwqxrylnr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gyzqndafl.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/ggiqfigyi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gxczzeizx.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gtvhnhzrh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtajvbzkh.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gohapemcu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gixgicxpn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gfagyseta.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtfovoubh.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gexcsjxep.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsgkumpbd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gdhxcganp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtjkffelh.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/goccypdbc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gorsxooma.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/glmhzdswe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gywunzpui.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gldnxoryv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gregzufnf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/graenqiqp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gtxnwbjfw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gprxohvtn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gkcmqnwcz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gwyjwgiry.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gmmsrsogs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gxsjxpksf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gedristjd.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/greqtyfoy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqobrubco.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gdxewfhep.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gpylxnotp.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gfccolfee.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gbisahqbq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gnqprwllq.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gmzsxgmyb.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gawtxktjs.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gfsvvbqib.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gwyfhtptu.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gvcxqkomj.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gwyqofcaq.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gxhyupuwq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gavitiqrm.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gxcrixvof.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gqaloumvp.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gquorisay.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gurzamxmy.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gnspdibts.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gttcsgkdq.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ghjbpmgor.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gwwwanfwz.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gbbyatqzx.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/ghpkipxhx.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gxbbmutyp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gcezotsci.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gvopaqcit.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gmxcutnhl.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gpyqjlujc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gfsuvgxeo.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gwpzsjqlg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/guolfgqtz.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gkwtwwqmd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/ginemsebt.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gtenfokak.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gpirhhkyx.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gwuaxvysy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gkzskkbsq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gpupaqwss.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gxuudvlwb.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gzbryybkf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gckgsuunt.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gmraqcsdt.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gabypvssu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/glcjlmfro.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gyyfacoel.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/ggfgjyjqf.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gybangyda.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gfgmtvthq.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gujokmexv.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gkazqoeah.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gobopiusf.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/glbofmvfz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gozodvgae.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gwaocpvhc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gstkytsxg.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gcmbmfpid.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gtdphlywp.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gakdpmzou.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gykytfphf.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gtmmoudlb.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gfwmsivyb.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gdhofeyph.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gaioxvojp.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/garzatpqd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/galdhmspf.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gxmocxnrt.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gmjfehncw.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gcamzyzlu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gqtvnhwop.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/glbfjbzen.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/giteijrcz.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gmmmbgswl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gduocetwx.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gummvferz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gyjxwdcuz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gilylhkxl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gnxvkpquk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gidoetuvb.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gnuqtyikl.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gypkfqswu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gyfwrcbkj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gmutbgbwa.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gpdbljqmd.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gehrheejq.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gkgmdvefb.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/ggiiltutd.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gwacviuee.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gmdzknhmc.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gsbifnjsr.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gtqvgpepr.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gzoteszja.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gdiqppzex.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gydphbzms.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gdttxrmpm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gxltwhyzr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/guzvtqxpg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gjjwgnvgy.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gizdofhyq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzdzhowfb.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gvydhrhfp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ggajlifvj.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/guguilwct.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gxdtsqeld.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/glhtpbfqq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gfktuxbrb.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gzokueute.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/ggbndndkx.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/guiuoyulp.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gppbdhpfh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/ghhyjqxza.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gecgdwvox.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gyhmbwlen.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbvilasbb.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gubkuibte.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gqqusovco.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/ghntlebfv.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gsglognzm.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gzapjfgek.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gmgxdfeaa.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gdvmisbse.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/grointfru.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gcmtasrlc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gzbxhszja.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gbgyoortg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gktdwejpo.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/ghwjhnvnk.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gtqkwhlzf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gukmicegn.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gxvtdnnmu.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gsevmlnie.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gcojkxtub.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gtuwctobv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gagubrcml.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gdkewriko.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gewsjbnwf.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gkchhqejg.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gtgbngkwk.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gbivyunai.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gxyehfwgw.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/grzptweao.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gwfhihonu.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gtsfmnzay.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gznogiyow.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gfsnenssk.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/ghneoylxh.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gxrpaluka.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gqzzunher.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gkxggkhap.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/ghedkwgia.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/grncaisok.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gcgtwhvum.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/ghspktyvz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gnusdieea.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gkglondee.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gpgndvdig.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gnjjoxeqc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gafzkurxv.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gdvmanjwh.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/giskgllwx.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gsmqzeozu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gvifpnknn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpptphz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gjvdnpyjy.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gyonfuwgv.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gfqzfmqny.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcugchfyu.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/grkorklek.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsnqagetv.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/geczqfiad.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gjqdhijbs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/guooqicfr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gedrvcrpq.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gomauuafk.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/ggvkelccm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gzobavzdq.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gytdyywur.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gmvhkpwxx.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gtfagghcg.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/guomkkvre.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gppfyjxjn.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gcagloyek.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gchayvmij.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gglokqwvi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gffaagwqr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gxowafltz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gbuomrwih.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gfvprdhxz.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gkgepiytc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gdldnwqqt.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gsxrfgfte.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/geukcekbm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gstlhgtrg.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gdjzjzbvd.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gfthfbatz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gkybqznxz.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gmezvlble.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gmonfszme.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gazjjhugj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gpikmgwzb.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/glrgtonpm.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gzdjtmwso.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gqzrigcfy.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gkwiwzapw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gywkktjyt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gatdrbtoe.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gfwihypjf.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gmvuwyhto.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gfemmekwr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/goqbwvqvk.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gqlyvznyn.sHtML


<!-- 参考信息 -->