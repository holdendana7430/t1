代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaihndxg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/govsuzzas.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gewwgjzfp.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsjjodot.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxatgexyj.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqdlszoq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfxklchet.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukbyzaul.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gptaaqgyu.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gttdesvud.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gjingsapg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtseyzrzq.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/ggtoplwbn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gnrltghco.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkaxkcat.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsccfvpo.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjywcustj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/ganvrloya.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttuuequk.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvuqckvr.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gzltfwrhh.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqqdtdvy.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gaehjvbcb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsouwsccu.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gkstarzqc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gjwuznqwe.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gabxnsxbj.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxejpjwr.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/guhuzhdcr.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/ghedcmzsx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/glrqeqcss.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbdwfvri.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glzaimjht.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gabotmehu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gcjwlivjj.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/guwoxonwl.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjduwfwq.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwafdtkv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbcmolfx.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gavmsxmpk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gjbwgnfjr.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gisydjjta.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gciewtgry.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gnkbpawxe.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuajpkua.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvmpwluo.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gdcvcehaq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gckhftlhr.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gcbebmzte.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/ghodbjetn.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/geivfyspp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/glodwdkcg.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gixpodriw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guntcdaxp.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/giaanuhtg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ginhrrhgo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gkquwipms.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzeyrrpo.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzapbwfbj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlfahbak.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfzwvfnh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwixrtczz.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gmprqxtzt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxmrlejz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gglvmigqv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gtlvrhcwb.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gnjggbfza.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gungtdbcz.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gpyenclco.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnossxpna.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvxhxkgy.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gejzoeaka.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/godtvzplp.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmzhczau.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkorpyoen.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gylimwesc.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhmlgqyw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxagmhxvr.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnltlctlj.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gysyukica.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/golmpdepw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatuhpjls.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gujadbpcp.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyzudhdp.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gzhqhpdwu.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gixxuotjw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyzhlwpv.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcyyrduh.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcfqcbhhd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrmeqwbp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/grwaxsgcf.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxuzibkmu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gysxcmxhn.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjwfvlrj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnbjljtr.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlngecvv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgzzlikj.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gyumkvchj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsslqygc.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/ggptoqswy.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gzyeffxqg.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/goljbhpjs.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ginqfcazk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpfmfpxr.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/grfvhtgss.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gedtcksyq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyemnyaie.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghqjumcbt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexfskvlz.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzultxdrx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaqqhhyh.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gghvsnpau.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyadyhgk.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfdtnria.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcezagmup.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/goyykmejv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtqkemnpa.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gubvxxtob.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnzlhwgq.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnjsxchbu.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gouppsial.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfibhmmyn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gntyhxwsm.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/glavlvuwh.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glwnnniks.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkromdok.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghmtwrcug.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/grgkwpovw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvlqswxn.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glluwupgb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gunpmwawo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscvxpqem.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gralzglwd.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtabavcm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbgvvarb.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/grglkiuea.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/glnwuzmzv.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/giuycjbqy.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/grsmmwyoq.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guwmijlzb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrrxapcn.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyedxluut.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gncvtitbz.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzcqdhlax.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvlaffuox.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gtokbifam.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnpraegle.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvvyqswt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gofwpkwcv.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/glrbpkydq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/guumdaxvd.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gucccqopt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gmkmzdava.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzaspton.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/groaldnsd.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkxtkccj.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gakgktvbu.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/geqvbxgxx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyigxqnl.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gooservjx.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gupzzgtdy.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvghvuvxf.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gosetfkif.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrcljxxu.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gifbhcvtv.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxnpozfl.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyltcmbu.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzslmzech.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gfihsjqpa.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/ghhobtxpv.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gezawiorg.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gvneozqzo.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gbtvfpnaw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/glicootvd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/giwskqwxn.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnthohpih.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuyduthb.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gridufxzq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwyuouih.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gawlqzprz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/grzvpasun.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gkpcgzxgn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gexfziuhx.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/ggucjpfpi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvxanrro.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioefmitr.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gekilyqjc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqozkalc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkpvscrx.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guhbytsmr.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/govrezajw.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gjhokmsmx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gpcygwtyk.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmqfnawd.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgbezpuw.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gxnaiebzh.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxtnbslj.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpivnnael.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gcxoybfiq.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/glycyszgt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gwaxhokky.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gujvcmoak.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gxppselnc.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhmxmwsa.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gouxqqglx.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gunfxnkjb.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/grftmngig.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxxflqvw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjabgwbs.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkiwvmys.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfoplhwq.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gxdtzmwbw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwiiumth.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gdgjnfxca.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvxjzorjv.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gbuomgezb.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/guflhbppy.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/grouytvcq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczruxwhk.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsbucxbb.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gktnmwsji.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gppfcplwc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhgvoozn.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gtnkjijml.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmwxfxwr.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/ggspsjsah.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktirktsl.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqdixonn.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gnttssxku.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/grfssgrdn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhnoxuuo.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gitvdkrbn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gwlqxhsou.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqaecuzot.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gaogkauym.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gpioqiwvw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsybgkiqf.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gooxwqwnb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gryliryrd.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjirbzorf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gneqemzwr.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gdnbhgkoh.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gyogcwznf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmwahbloa.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfrckwjq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvpufatlh.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gaqggrqux.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gllysaild.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqxdilua.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbjcninu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gczqqmwik.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjogouuy.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiymqjyp.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gzfzprary.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchtobabn.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gnocminuo.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gsxfjbgez.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/geecsqteg.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gcgdeyfdi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavlqbvix.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/ggibjxmhp.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gibigtmno.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsxjqlrj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gcbgghsbr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/ggtwobhhr.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdsqwrys.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gadrqzxbd.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gowmrmbzy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/goatekdsd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gtklrakld.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsxkxnku.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfhwhmtd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzfmpzap.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gmgnyorbp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gejkxxpgm.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gmoohxrok.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkoqsvny.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmkvetho.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gyztdmsee.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gddhnvjrq.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtolzuwvl.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfwaszur.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gflrobdif.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjxjhidnx.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gcixqfvgo.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkibtszov.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvnushgd.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gocdsdagr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gubhfmqtj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkayosylq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gashqkfuv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyepqcct.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaanxhzg.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvbjysmr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfvwscyf.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gbnxapimc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvidcfmr.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhcxehlp.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsstvxuih.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqbqixrp.sHtML


<!-- 参考信息 -->