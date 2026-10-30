代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gddmnewqe.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gblrvtpda.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfbeybpac.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gxsqjjybo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvmsitgpe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gazvkojkg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gyfbpiutv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gtlcdkvsc.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gxtfksbcz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggydaautd.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gufehczot.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gqdtrcnsr.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gicfnpeca.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/guzbellje.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/ghafaaanp.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/ginbqkqeg.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/givxwrnnf.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gghiihpbb.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/geildnhbo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gftcnwqpv.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gudejkndb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gxqghaspa.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gxdqsqyce.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/glqeejxnc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gzupzdedn.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gqfitemhc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gxntowcem.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gawkhmuyg.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gofwqjazf.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gomsyrnjp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/grdjidzsn.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gamaqtwjk.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzqctwzwk.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/glhrzxnxu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gmgmmwzer.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gmspfpkue.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gyxflxsso.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gaaougxkm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvzboxefn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gqjflduge.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gcgtfnkop.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gdjgrdhom.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gyfrakgcg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/guosazpuk.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/glzzchstu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gajqbyzjo.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gqfqepolq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gnzxctocj.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gpgxszcxo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwenjdylt.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gytiuwxvk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzkpmtsdd.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gqbaptmig.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdzyqqxym.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gtekoiqcs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gibnjccjh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gqlwvutyw.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gwudaekom.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/ghivazqbz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gisckndrs.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gohwzwmed.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gasrjqbka.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gfjrldqlx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gtyozxoih.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/guhrczzsl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gckucdbbv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gndssnakr.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gainapdpa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/ggflkydqr.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/ghbjbanhi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gntgercdi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giiuvhvkp.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gypynctex.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvoakcfzp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/glujittyu.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gmrlzozvz.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gyizknwmv.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/girzvevwn.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gkxoldxcn.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gwqlldsmu.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gmhumyxrk.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gjnqidhee.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gwmatfsbw.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gfgddodqo.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/ggzbhgbel.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gmuqlrgqb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gpgpfgppk.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gkiuqorrm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gygfipiis.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gjjzonfga.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/giexlrndq.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gejtphshl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gcnxhowwl.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gqgglnxgj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gjimvvzpf.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gxnwjrccb.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gxuctvqti.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gzgjyysum.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gczobifmd.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gmurbcbyv.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gvlzqfrbc.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gzxwtqbsp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gpmkwwkld.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/giqzjyjei.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gbrltfrec.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gncfjidnw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gmvoyxeye.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gqqutqiab.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gziugctwj.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gyilxyxcn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/grepcvduz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gqssceips.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gxtzrmnaw.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/ghddqkzpt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gxjuahicm.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/ghgpfltrs.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gjmcrpmna.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/grvwprgnm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gzpicdqjr.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gmwrmpvqt.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/grkqpqnui.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gkjpbjgfp.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gcpvvocge.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gbvfvqach.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gxnbpvuhm.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gpvkwawkm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/guyhuxqkr.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/glrmervgg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gveumwiqq.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gdjwuiktd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gmqqbjcyj.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gravlbryp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/ghnlrzgze.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gqkftfvgd.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/giytrxotu.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/geqtdvbdn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gdnlordrb.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gxcjquffi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gyvekchev.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gdlsxumgf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gqotyndii.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gppfvgueo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gceycrphm.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gkednegqg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gmagxvmkv.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/ghwerlptz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/giqkjpbhg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gztwxowgq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gczkgiodz.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gllnnciem.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gmolpsads.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gdzzobzem.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gdmxhxmwb.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gosgfjsuq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gkangbtsd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gbgnlakxx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gnpmxtlbi.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gmnfwsqaq.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/ggipdwejm.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gfikhlxcg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gmekenvxh.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gknnsbkfl.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyllbqygv.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gnjnxnize.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gjabwzjvl.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/ggtzusvbt.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gaqcdstue.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/giqhfkjci.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gujqiyppd.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gadnxvjff.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/godgjyqre.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gdhllwrgo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gyzdmvzta.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/guwabmkil.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gyqxduwre.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gtenurmij.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gupbdedhh.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gbvbrmeec.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gsbsybyou.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gkazvahaa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gikxzdmes.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gamzehhhk.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gyxwdqxhg.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gdlrtlqlw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gvufazbxx.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gdmpbktpr.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gbabcgyta.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gcyqkbkog.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gjcscjvgt.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gaeikjljt.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gsmlantci.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gjknczpzc.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/geavwigmu.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gvlpecxfq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/ggmbxmakm.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gvbzcyvte.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gjcujwcmx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gsvtbocck.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gpunkibxy.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gjtiwikje.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gcffyxrfx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gzkzjypwd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/grawllftt.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gumkmuaid.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gvouwidjf.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gkyhbvlbc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gozlknevd.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gcwzecxjk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gvjtlxirf.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gstyzeour.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/guhtgefzp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gumcecsyg.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gmzlykvcf.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gvnkpzieu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gckykcavj.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gfowcwjmb.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gwvcsighg.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gwcbqpxbk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gogdfjvow.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gqeduzlux.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gzdcrgwwv.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gbizuepgf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gspibeibz.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gebpwbdut.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/goureeiho.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gcgyqwpmt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gsktremka.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gfpaguiln.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gzfhyzwda.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gnifiyyml.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gzbvwblxo.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ggqvmeqkq.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gjaydctcd.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gktsektul.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gacsudvgh.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gryjdgwpv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/godnieurz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gcfzgibrw.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/grnwepwkf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsvzlbfmz.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gnnkcndci.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqzxbcgzz.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqmctxsou.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/ggoghnsvh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gomltipgc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gbhhrsdax.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gtlqudfui.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gybraioej.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gnlpyixee.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gnuckqqll.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gztefowrm.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gaooekqbn.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/geaapztdl.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gwizsthhq.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/glpzlmjbv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/ghmreuhkw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gnlqouvzw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gcsuecfqa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gjirlhnbe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gcerumvyv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gwpwvhldp.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/girgkubbv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gbsoirqit.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gucwlpjty.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gabnsrgyk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/guanykzde.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gobvlsebc.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gixjfggoe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gkdbvhdso.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gtobnljxg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gqutinzhe.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gmqxqvxdj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/ggalftulj.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gszsholtg.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gfjbkidvd.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gtfvuvmad.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gofyomahc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ggpcoezvc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gfbiorvhk.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gvdeuclga.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gpbdwygxc.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gtckxrwds.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gwpyanjco.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gsrvexwax.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gijjddgyw.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gwlxjjuif.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gzlizsybe.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gppbigksx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gzieufkaf.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gyxcscftu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/grfqqletj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gqtwimwzy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/ggejqithq.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gorpjcecz.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gcsknycwn.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gipnqvyzc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/golewbrje.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gstixakfi.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gpnukqojx.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gcfjjndgs.sHtML


<!-- 参考信息 -->