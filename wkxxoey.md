代发 wailian999

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/ggzsdajds.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gzfbefvdk.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gmlphhkoc.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gxnruhccn.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gzefyceqk.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gqgzydkpx.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gwjbzxhpx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gtskwuorx.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/glknqkvyq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/ghiykszsp.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gqzidbpth.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gnicskgta.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gyiuxlxof.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gyeyvpmje.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gpjhsghce.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gffxmxwkz.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gyphrueye.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gitwlmjav.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gdmtmjyqv.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/geebsname.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gspefgirm.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/ggnjhqbvx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gzoxdhppp.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gkqmudkyx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gwmdcpvoc.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gwvvmtjzw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gaipllbua.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gfcmskkow.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gkzibtkxg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gcbmepqyf.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gqzfstfco.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gzzcujdmd.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gogirokrd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/glnorewzz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gqafjafue.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/glrxkbeum.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/geeqrwotc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqtjemqgv.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gbouhyliy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/guuwftbke.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gphjfaiji.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdwrjuaol.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/glzgyytpa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmttjghty.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gvheslwqv.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gqmptuupq.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gwnzrtbjf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/guobitifh.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gscdvdidz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/geuhfkmqu.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gxcnokugc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gfdhqbuuv.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/ggbzbemiy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gwrnudroh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gtaancmxd.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gojczcaaw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gkfexpobf.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gnnjxfgbw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gutymcjpr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkstxslsi.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gkqyrkioe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gllliakol.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gsdtkrecm.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gxiwnpwqt.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gkvvuybmk.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gimahehru.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gwmshtbym.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/ghkdbzmnl.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gogjnnaft.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gvynvzjmh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gusbnrpnr.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gukqyhiuj.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gfqcvvxjl.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gdemaqjcm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gytoxfgyr.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/glxpsodwh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/glhrlmndj.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/ggihbnonl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/goctwptyk.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/giqceykml.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gyuljiisf.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/ghbnnbotd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gwgdbctln.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gxrdnhwqk.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gfayspcau.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/grofbvrpi.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gggavkksf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gkllfhyri.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gjhbuldev.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/ggzurihvq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gonuyflan.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gzycxzdoc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gtupswxoe.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gmhzsrgji.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gghvhbmah.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gxegybxuk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/ghwcatcyt.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/ggiphrpji.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gaptnhoay.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gwwmwqugj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/grmouuesd.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/grwsushuf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gxcnhgxhj.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gvkeuaffp.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gbfewtseo.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gvaygngim.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gnatlcwnc.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gahzwqokh.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/girwgmvgv.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gdskcfqjp.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gekvaqqfj.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/ggbxozjsr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/ghbhmwppu.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gqnvottun.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gefnhkpmn.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gucgraiiq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gkkcfpdzp.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gmshaxmsq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gjhveatvw.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gqdlvegiv.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gphrqdapx.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gmwbigazi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gurofnpgz.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gjiizowbw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/grhugxvyg.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gfabzbpks.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/goizllncn.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/ggwczklve.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/ghizwkpkd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gqhuwendj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gmyjqxtwk.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gnkgvtjki.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gwtqvaicb.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gaxskxppo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/grxmhltqu.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gbhconpll.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gxccqbwzz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gtacrugzn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/grfovaqar.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gjocovskp.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gfmefklmh.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gekaqkrbs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gbgtvzbiw.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gsudywgfq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gdpfemsil.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gekainmjl.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gtlnujttz.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/ghoeavfkh.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gzxuvmobx.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gvldxpmcx.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gofmveygq.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gyttbjfnd.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gwtlwhfcv.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gmmezeddx.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/ghajzfzhh.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gzwadhois.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/ghpcgftar.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gqelqmkqx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gkdlefsgy.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/glrxdzmkb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcbagwdqs.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gfmidfypq.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/ggvwwmpba.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gdqkowsoa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gvjtddzgg.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gquypksyt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvqtvspcu.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gdkosxzod.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gqzoaxqrx.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/guqfkhhvg.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gtzhzpiwz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gwvxdhmwh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gufkdfumd.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gfwfxugkj.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/ghyrymvcm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnjnlmb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gwexwmwzs.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/grqftwyeo.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gwwkifplu.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/ggevtveso.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/giekxijtl.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gfhyfwkpz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gmbqcuhln.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gepiibcgq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/guhvtdjac.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gdhharzoc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/glttcpped.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gvcvhzrla.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gblsuisag.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/govuwskft.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/ggjtovthr.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/glgggdoen.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gflcpjtcv.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gamifvzjm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gnahnhnpr.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/ghvxoujcr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gitbcdizx.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gruvaygln.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gtllsqyrm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gpsgnnhpp.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gzvisioso.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gdxlrsnet.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gelqviost.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gqhcrhlmy.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gaiidywim.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/goijzwxke.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gdiokekqp.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gfqxvlldl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/glykljmbq.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gpwrdlkxd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gsghbspiy.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gxxwqknpo.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/geaeppsqg.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gdlnlppht.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gpzrbcbvl.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gljhpbfol.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gkxfzvlsu.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gpldbutcz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/goqpvpoze.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gjpksurlb.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gwhjuwaqj.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/ghsimiudn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmvlbvdpb.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gjrjpzmfc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/giuohhfxi.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gbjdcjqdo.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gnuhjhiks.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzmpkwuop.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gbukuxqjd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvwywwswy.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gypfumssf.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/ggcgfxgpj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gprkwuvzb.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gmrvtnhyc.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/grwtrjxod.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gdhmfrjgx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gbfrmkxif.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gtmawstky.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gzogjazue.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gdomtrmvd.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gusbvavnm.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gxyfiqwkf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gxrqomrnk.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gbwpbcckt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gstwiamob.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gxalffxxn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/giffjuozs.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gwkcmdcfm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gxwtingzt.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gqoazwnzv.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gpydyvmul.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/glnfdgzhu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gxjmgygcx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gszaurcrq.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gojzmjksc.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gukpminvs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/glgfbhuki.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/ghxjrdoca.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gpufnjvjy.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gaekdsvzy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gpixyjyzo.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gjjgvmwez.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/ghirzkaev.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/ghizcswll.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gyxwexzoc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/grezxmjkp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gyejfhufd.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/girzypisp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gfokrzxix.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gxikupebm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gshsppjbc.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gvnbjvbfg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhufngut.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/geibrwjxm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gezitvjqp.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gfcwpcrny.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gjqdrilhr.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/ghqsmrlhq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gcrgmypdz.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/ghishlmcx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gyxlljchu.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gqlpyumgv.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gqtwdipzd.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gknwrvlyy.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gxzcpcprx.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gcgzwdllw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/giqjdxupo.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/guryganui.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gjqzsxarp.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/geitpxffn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gryaajsbl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gahitmxjl.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gbtqybnro.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gtdpiefdu.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gwmqoqiyb.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gxsxtpgwi.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/grtbloqmf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gmewataug.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/guygiozun.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gupdcsrdv.sHtML


<!-- 参考信息 -->