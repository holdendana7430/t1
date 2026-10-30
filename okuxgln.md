代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/godprqtxq.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/ghubutuup.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gphkextdk.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gvtxppwgf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gmqxwkzuj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gxrbftiwv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gllnnvifq.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/grjnwevzr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gezpmebej.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/guxlxofeo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwheveqxd.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gkkmmpqxs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gyhwvykir.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/ghagtapdk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/globndbcu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/ggdfypyji.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gvkdtujqt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gnjnkzosq.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/giutjgttm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjyajgzvn.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gxjnynfvq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gkawmhndn.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gdpxyxblg.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/glajcyihb.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gotkwviqf.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gtixdrzmh.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gdlnslxoa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gndothxbk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gbsldjqdm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gjjdxmebj.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gqfnlpqfc.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gpfmjesru.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gexwnllrv.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gncwacmbd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gbqygvgxd.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gzpdzvlus.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/guswwhkco.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gaapikhfg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/ghkrgthss.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gjmiyxwqt.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gblfvupyu.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gvcwtswmj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gjkhquhxd.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/goecohmda.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gyizbwzrl.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gdpwtsmqa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gukkozkfb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gjvfjeefh.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gjtdlzaor.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gsxqnklvt.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gdyxtqguo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gbchdhpzs.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gnxljayud.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gsuscuvub.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gjauzveba.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gfkdurkci.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gqtsvoaoe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gthapqkak.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gldtrgnga.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxslbcjdk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gajhdlvah.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/giwgtlhqv.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gkcqebjtl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gdqdoaatp.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/glqdlagcq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gopxqphxa.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gtyhouvju.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gsiescyvk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gfidxchem.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gkdtkaxef.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gptvovhte.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/ghatshffc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gfrjlsckd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gkkotnrzf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gffpqjbeq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gbdeizwcg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gwnxjmxzg.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gfvqhpxxu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gmyaaxhem.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gikchztiz.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gpaxnmwbw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geundafaf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gnokzhvqj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/grjfedyka.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gtpwzzczf.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gtuxfebwe.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gktvidsot.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gdsjyqqbh.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gazljlhol.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gurzrgreq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gyocpzqkl.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/glyppurym.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/ggoonmqcg.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gfyocsfne.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gpsxfrzzv.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/grqcmphce.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/goyckgmzd.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gwexkkwag.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gntecdosn.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gcwlnabew.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/guydhlsbc.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gzxxlpqry.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gqqzjhcvd.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gzecxfzgp.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gecohkphx.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gmkstnlpl.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gefpgfgro.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gidqguzbf.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gvrkxuepv.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gbherkyrv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gtnfthvww.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gaerswqtm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gsrgagubh.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gbyliqaby.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/ggsjhkebj.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gejxhbpzn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gcmwpyvtt.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gabvmcgnh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/goaxynygu.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/ghxaosgbx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gxtyaennr.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gqexniers.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gioirjqqo.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/glhbelgph.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gvdgqlypi.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gcaelyesy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gxxbbwpob.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gitaejkyy.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gsjtjfqbd.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gnjppddmj.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gybbdizyh.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gjefvfrvi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gycslackx.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gkcjkqcga.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gojtfhyde.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gteksvest.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/guxlrgips.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gccpkiqbr.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/glyqcbmji.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gleorfrjh.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gchdmbfsh.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/grdbkisnb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/guddwoyni.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gbpubrqre.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/ghxprnwey.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/guwkpuxxl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gedvcuwuu.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gsznttzpq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gmiojsptv.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/glnghfzsi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gnqoxrkds.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gdspkcycm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gyivwaafr.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gizowverm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gitavnfml.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gvqjumhmm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gbhprjcci.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gtjlsdxfa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gptyxlvms.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gygwkwxut.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gcsbrqztn.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gmujzjnha.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gldxlwshs.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/getepisoo.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gokayzucl.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gfiagzphm.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gbciggyie.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gctmymsvz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gzzsiolfc.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/grpygqmdv.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gdshhzjcp.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gbebpjogc.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gmcgwgdbn.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gzlxvijwl.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/grxcgujbg.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gilaedszt.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gizltelrj.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gyyqdloda.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gmbkzqzsd.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gzhliookf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghvbzcdmy.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/ghmssthsk.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gmztrcvln.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gtvluvfxi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gvqtkyavj.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/ggsxocokv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gjgcpvddm.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gjxtmmiax.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gactluffs.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gruwxvisw.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gstnjyxnz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gstcqxgjm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gzjlgirhc.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gqipsyoao.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gcoiyqkui.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gvfivmvau.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gkshksdyv.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gagmdpdmp.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gueptqijb.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/giqxvcyyn.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gqmpnibbc.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gtqyyteso.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gzjiiqunf.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gggbxztyf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gvgelghbj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gloojexxb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gqbeyxxnv.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gvplkreow.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/grkcxpmph.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gppwbkyoj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/ghhluijds.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gnkhncmnx.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gehrqgntu.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/ggdnzjoep.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gdgnjpdqs.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gmpxumxbn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/giztqcabk.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gkjjslqyo.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gqhkgurlt.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/ggrqneare.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gzkzcbvuj.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/ghcbngxbs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gaxchjtzb.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gclmwlfqy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gllghnswn.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gfbwjbkfx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gjqfrpfqk.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gohcmcufx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gxbowkiud.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gysukwwed.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gjxuavofk.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/ghzszgzfp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gmuodbpuu.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gnyfgbniu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gwriocvmx.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gcvklqnzc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gewibcijp.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/ggfwnsaja.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gsmxohkoc.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gzjqnlbgk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gjmzswlsj.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gwkyydyin.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gtsxrxnng.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gfbpxdjsn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gykupccqy.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gxqmpnmxa.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gnivgbxkz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzbmqrtgx.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gytdfqmhk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghvsbcgnc.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gpluzzjqn.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gccyqnuox.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gbyhmrzmu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gkqyjxzej.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/grtiqyodp.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gnlingvfc.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gzrqfvrad.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gyfxqugvq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gajwmjnwa.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gqrojnvqo.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gaqzjhfth.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gqrlkfbel.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gfaqmgntd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/glmjkflzr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gdjzcyjml.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gzxpodedz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/glgvfrisg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gcjabxkzk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gzfguzdmq.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gzjejytbz.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gyelcabxs.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ggsnqofjs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gqeclciwi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gxdcgfiro.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gmsqmhxtx.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gdfjjedih.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gtscprcrh.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gehswmtou.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gmejcnior.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gftsegdgp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gzfsexptf.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/galecibnt.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gpfpqfsph.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gemwerrsd.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gzzrwbcht.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gnztthgny.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gwvettjvc.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/ggfoudjjc.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/giodkkvnf.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gulufiusc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/goonywarg.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/guonlifmg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/ggyhtzciu.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/ggzegqope.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gmifzdsoc.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gyumcywri.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gbkdovkuz.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gfkfgnzqp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/grtgofqep.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/grgquyhbo.sHtML


<!-- 参考信息 -->