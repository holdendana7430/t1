代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gpnntyjpc.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gtrcjvbgk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbsiyrozj.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gvrfzxkgg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gudxxursg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gwlylrare.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gbhlbhctg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gotbpwpkp.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gobdvzqiw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gikziavdq.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/glzvavrsy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gbaguhkba.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gwspbhqqr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gqxrjplcu.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/geoysjpck.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gfwzkpsok.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gptswaokb.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/grsplukcs.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gdjrgfvwx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gnojrlcdp.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/ghnjjmosu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gwsqtsret.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/goprtogcp.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/glpdkiiqf.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/ggxfotiwd.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gbgfsfoql.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gikbfkytx.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/glbepdsot.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gnoqcebvy.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gezpeseav.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gpulfzsfo.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gfhcwnrvj.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gxwonyeiq.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gnaxxjyvv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gvuovwmeg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gyjtbiywj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gvotksets.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gxiqxoepk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gcnhvcaqn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gmejpsobt.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/geycludiy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gksdcnaec.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gahzcgsfa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gqktvkdpo.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/goslvkqcn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gybtnlkta.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/grrrzxdqo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/ghzbjraha.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/guqyrkyww.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwdevphto.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gnihxwqbs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gyzesywoe.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/ggpnnauxq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/grahuabou.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gsogjrayc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gskujyqip.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gguxyqolp.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gfhyzrcqj.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gxwyrygqj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gbqtnxlpj.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gbhodxrqt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gimyehldn.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gagpvcctm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/ghxeoaojy.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gnzdfjlyi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/girhwxabb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnooememz.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gusvattln.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gqpkhmztd.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gxaadjeuc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gdfcaryvh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glhwfcmlu.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gtjktnvce.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gezdgoman.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gcsarnpto.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/ghavbdhae.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gbkuuzquy.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gqmutwdnv.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gehbzjpro.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/geiahwedb.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gsvqayfhx.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gxmnvvnew.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gkwqffmsh.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gkcpbohrc.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gcbbqkjqe.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gguzcvmty.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gcmgjdaag.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gzaflsosq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gdqlsotsu.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gmiulegwg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gzprxcfuw.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gwdwwezic.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gjfpwkdlx.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gacycfdsj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/ggqxeysyk.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/ggkpfjmtw.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gcrevlpai.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gtbvknvmv.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmhhnjarl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gdckyxxka.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gnahrbfrn.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gaoyafzsz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gfuhjajbz.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gdgsvdlni.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gbcndjsif.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gctbddiyj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/goghwmrte.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ggwvpusul.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gatixffgs.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gawjnywct.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gyichmdyp.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gsavxaweb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/govcmcubu.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gxxlapsoz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gmtewjbrj.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gzduxopcr.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/ggksuvakt.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/geysrwtkr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gxmbhubua.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gmohbfuvl.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gosefewdm.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gyjueuvpg.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/ghsyjdeev.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gykiusvsc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gidrdhezi.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gltbgummk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gukhlsipd.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gnrqonrje.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gfxztlgfu.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gmjuoppyc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gcttyhpda.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gjeccelgm.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gbjjprshl.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/ginadfwww.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gfigrvztc.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gkocrqsxi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gqpgzfngt.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gpwjhrxhk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gxabihkvm.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gushnuexu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzmzvyqia.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gihjctohr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gylqjpzbk.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gagyrcfye.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gkvubbszb.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gtfgekbnr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gendwvovz.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gvpmdhxpl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gcgypejfn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/ggfjptvqs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gettazena.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gwoubzuij.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gmlquukdf.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/ghrxffioz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gnfjqmexp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gihevymkp.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/ggjeppvvr.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/glkxpidcu.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/ggdmwpfns.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/ghhabsjcj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gjhmqhyqh.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/ghpivdsgi.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gqmamzkev.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gxpkubdpy.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gudokkozj.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gmfjxlizk.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gitbmukgr.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/geiaekphx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gercbzcvi.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gcqcwcopn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gjoansbuq.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/grwvtfoxt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdkttjpoa.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/geufgzywf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjhegjxlj.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gsbekcblc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gssltdzet.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gppawwiwc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/grdnbvscp.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gtstpvzka.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gmkipgpxv.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gipvcvihm.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gaejozhmx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/grotxwkyy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gplhblahg.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gaxkimdsp.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gyccmmsmx.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gdwbjmlqz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gmbepasxy.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gawpduxur.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gatjgzqux.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gpbhhtege.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gewfwsstb.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gzjrxbfvn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gmarlowbc.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gvyejbeia.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/ggxqkgqgn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gofxfpqta.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gapxxvzdf.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/glvpxxrtp.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gvoxmvsra.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gocfymtvh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gjmfjcrkx.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gzhuenduw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/ghcfvhorc.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gyuucdtyf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/ggshjropg.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gcotnygou.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/ghvtwsopn.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gwtjctucr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gwuzuarit.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gokanvehy.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gpslulrcw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/goxvqucdb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gmdbqyjya.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gwkdfskfp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gfuvixlmm.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gidbemnqb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/ggxgadpmk.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gdsqcktgm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gqyjimedt.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gkrncvsou.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/ganhtmbnr.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gsedbpfgv.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/ghundoxex.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gopudbcji.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/guuqhkxhn.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gaofhmjvh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/guscgvtrn.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gkzwiynzi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gaouozgsv.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gyoqhomxz.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gwqxkxrxi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gjpcucxty.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gbrvylpzc.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/grydsevco.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gqhvrsnzs.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gxappzngc.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gxdlppjxj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpffdggis.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gdmaogfwu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grudnioiy.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gufoncirk.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gomyoqhga.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gbakvwdak.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gtoewqphx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gkonyshel.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gjwmiwgjz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gqobqivbn.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gdoyyjnyy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gwcxbmvxe.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/glfruqixb.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/ghhezfrbu.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gkjavyptt.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gyllxgxzd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/giblzfspf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/grxnvwmua.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/glkjoddpo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gmwapabtg.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gofiywasv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/glolffcnu.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gjokmhzxx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gkfprawxl.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdpkaxhkc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gkdxexzoc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gtfajghbh.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gctzxqjhi.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/guawrdaew.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/ghwwtkkbq.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gynpcwtef.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gbvzplpta.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gpfnezvzn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gptusxezr.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gnnqrmjmo.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gqrmsugbm.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gkucdsbrr.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/goattbklz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/geaygxbvd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gbcqyxuvk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/guetkpkmq.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gvhpwffqc.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/grdhrvrpp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gjxaaxjus.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gijtxqrfg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gnczsjqqz.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gzvfbunrf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/grcssumak.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gcsifvgsv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gxmrhysjz.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gwitcvzjz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gnqgqxgvc.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gzvptxkyt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gqwwfmiio.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/grbodekaz.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gfteipxlf.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gdbigyzno.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gqiybyemb.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gbwtcshdr.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gxdujchxr.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gtiimjekr.sHtML


<!-- 参考信息 -->