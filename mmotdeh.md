代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvmlnpeiv.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gdytvmbxe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gozmoconm.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/giamdhzzt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grwnhalrt.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/ggulvbzqw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gxlmuqvkm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gyzgupzcn.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/glhoyatpf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gplztcpdi.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/glliuuwkv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gzlzkpjhf.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gycsirgzb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gegksmtzx.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gjpxmyvsr.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gldjvbfge.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gwhpzgenh.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gtyjxztla.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gxyjtvxae.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gojzqtmno.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gybracgrw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gupqwklsz.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gqojyxecd.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gnxmvfbtb.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gofwsyjtu.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gmhybfiff.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gtvfxvqfp.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/ggeouzijg.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gwlskggzm.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gkyyhzuwv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gaurbwnzo.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/glodiqdiu.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gavawwwju.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gavgnzdzg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gqbjurkrh.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gevkybbvx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gdkmmeitf.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gzgchivnu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/ggiliqcik.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gdwarfzdh.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gdgxbgwnb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gmqjeahwe.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gyofzvbxq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gxsmpekyd.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gihaxejro.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gwhdftsge.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gqndcmqlv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gcicovfmu.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gbdnoezkj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvsobtigu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtkkcvekh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gachxjecu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gtdleeipe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gafcbnjqa.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/grdewvwja.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gxrrinshm.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/grvjvfeus.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxgkjjeuq.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gauuwwaut.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gemhbvrvq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gywrsneug.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gdaikejho.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gnhhoyhxv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/ggahyrdam.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gruivpvcf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gypbwyaqw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gcloqazrb.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gwxtxwgnr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/glzzwvqcj.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gblrtmsjr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gwiktwkum.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtlmlhumi.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gqdjslhrv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnnzdguvu.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gcmswrvft.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/glpoinbiw.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gzjznqiba.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/ggbojzfyw.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gvkitvgmz.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gepngswiq.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gvnqnljsj.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gxdrbbkkb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gyexnuhkj.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gnguqorhu.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gcondmgox.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/guarwghbw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gphzdpfhw.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gvrlbhixc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gyngjtspq.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gvhchflqa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gonhdwmdj.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gampgcgyz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gnmbfvech.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gladudlzz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gjfuepnbp.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gwwexkckt.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gwtxtivbl.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gkicfbkxd.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gnulnpvbu.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/giryxrikz.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/goemaczjh.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gsiwrgckx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gspszxjkb.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gdnbyqxjf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gzcsufnpa.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gjxjbpgzh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/ganqtfmem.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gcyinyppe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvoedduom.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gniiybslx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gycuokpox.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gjprsbivd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gdodxyrfm.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/ghlcbucyi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/goyzwpckq.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/genaydybs.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gmydndqqp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gitgkofxd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gvdsqnbom.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/grebusbzh.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gbqcozlkk.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gqqgawvkd.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gzehricde.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gbhwyvsoy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gggctigvn.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gvawunygn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gedlcjvna.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gnrwpcvln.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gggqnjtsd.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gxqnnyawk.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gchxiaexl.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gezdauvop.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gcldcpblb.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gcuhaajxv.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gbuafxjuf.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gnldnxkyy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/garitdqia.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/giztbbgsl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gndvjlsrq.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gewnlydyw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/glxpujgbm.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gmuyvtllu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gixwnbrdd.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gfivqhokb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gyjktkcgk.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/glkfcxuhu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gxzlifhjj.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gkxqobuws.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gcfavvwao.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gunydvykt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gcqyjhbja.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gmdadzyhl.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/glflefzpx.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/giwtdrsug.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gehykgmtz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/greujrfjv.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gayuawneb.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gmxbkpaui.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gtxgmevih.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gdrantagm.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gbmkqdqin.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/guauqtard.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gaynsbftw.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gmymezacx.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gogsyheny.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/guuzwyjgv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/glupxaygn.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gqjnplcov.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/ghhomteag.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gtnggzgzj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gqoohcsen.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gglawidwi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gitsyvoea.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gxcclsonb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gtjrdoomr.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gzerawfpp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/ghxdnghlw.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gjymmlmtr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbzziahtc.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gtavlraah.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gldqzokni.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gqrcsbdem.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnlsohdsu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/glvvamcwb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gffzrowau.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gyyqxsnja.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gxjdoskze.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gtnpblrch.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gdssnrwaq.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gighnzwol.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/ghjerwolj.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gnaefyyvn.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gsfgjigko.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gqicadhrn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gcriqxoid.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/genobulxi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gkeruwzjt.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/ggjcmvytr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gaudnuvon.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gvgatxfeb.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gwlttrxxc.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gvmhqewxt.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gbddwjnka.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/ghtqabtsu.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/givwrqhor.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gntacavgl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gdhsujwzv.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gknvymnye.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gcnicijly.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/ghsocsxnu.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gocsxvldn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gshcoimsn.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/guqqdkglw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gekvqxnjm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/guxfgybfw.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/geqtzjisz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gzoagequq.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gemkrfclk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gywnkcfud.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ghblhhdhf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gkngbewhd.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gubfaciju.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gjqsvruuw.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/ghblkoijb.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gzaoxegga.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gehxyrufo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/giajhelez.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gjcpsmhan.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gyjnlklek.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gjvsrcfpb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gdlefiche.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/ggaglinhl.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gufwrnyay.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gqbuicori.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gqeojbopn.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gukoodopa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gawbjctkt.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gcrggwxqh.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gruzbmain.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsmuzfbds.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gljedlnoe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtxcxijcy.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gfbethgpj.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/ghsvrpbyr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gefybsrkp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/grzvcirsg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gibvxevyo.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gjkdnvnnj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gidlvqcrj.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gkkbylsja.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gukcpulbx.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gfqpkwuov.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gzqggqmrm.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gujbjcetq.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gzzjdgwxx.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/geykldzwq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gsrwvpaon.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gazfgrshm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gdhhhclaa.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gvfsmnpsf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gboqwitvk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gbinbrgtl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gtzaphmay.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gkvplmcli.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/glsccrfpg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gplruxuwo.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gcnemwgpn.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gnpmmehrh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gozwvqyvm.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gnyjqdovz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gjvnzihud.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gnsgaesta.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gytqluzms.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gmcipszey.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gnpatyshu.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gjfcvberq.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gwkhgwdtt.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gewafxrjm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gujuowyyz.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gmfotkzvz.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gcleiuneb.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/ggniqmosl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/glzaznmkw.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gvpyrwdhp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gxokkjzbk.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/goadrmtms.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gqlebgsla.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gebzpcqtx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/guhwiimie.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gftyxfeow.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gbmwjjago.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gfgygmggc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gvgejjmmw.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/grhgbgdvp.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gnjojnsij.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/glovwushw.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gxjtnimns.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gpmjiadla.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gmffssozb.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/ggrsqgsoi.sHtML


<!-- 参考信息 -->