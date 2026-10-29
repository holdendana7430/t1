代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqqsxzedk.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/guncvzmtj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gfovhyqul.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/glrssuhkn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gijxbwdtz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gncbmblvw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gzvwfowil.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdzcxvbzc.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gfqjxzfcw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gvvllpbwf.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gayxubegb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gvuyqpmnf.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gfccnuvrr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gpjcsbrcz.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gbblhlkqe.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gfziuqbbb.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gunourxnv.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gqmnftqzk.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gmnpidpej.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gdqgbybjc.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gvzlkwfvu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/ghnqphbuz.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gdfkartcy.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gtneynzlg.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gmmbxldya.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gbnafvqoj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gkclzcism.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gfkoxlctp.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwnlszjhl.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gfmsmvyvj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gvxejxher.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gygioefqw.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gihefhevr.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gkzywpjlw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gfhuvjwjg.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/guwwkagzn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gkzmbutjh.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/glqcakswn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gseypipqh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gwjvtvdqx.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gwjvpljcz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gdejieanv.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/ghydhanjk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gupiohmly.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gunutyqml.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gajjhzlai.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/ginrisyla.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/ghltilcrv.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gnwnwolyz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkijmpzfy.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gmfkpuciw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyvvrddwv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gdahrfaqq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggriwdmtk.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/guwwavgux.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/geliygltx.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gbwkulsdb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grisjomkj.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gsmzxizga.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gmkhgcwog.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gohtuclqo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gtfvzdgxf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gwpgrollu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/ghykimpxu.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gglkknnzt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gnjtvuwmr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gogntbfkq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gdzwgzrkz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gpdrnxbnh.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/glywsciae.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gfhdywfit.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghsxhdgus.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/ggklwvgll.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gudftoqeo.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gjbdykdmi.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gnwdfvgwq.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gteejuxvh.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gxqvwsclq.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gbugqfcco.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gyvbxxciw.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gvyhgxvji.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gfjqeilsi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gkrasghbc.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/grvmvvfba.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gftsavbhr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gldxclknm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/grqcxtixq.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/ghlplulay.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gidxxmcrn.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gehsfpyec.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwytvxyka.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gfkciqidv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gplbxvktm.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gjkewqysw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/guntqwubi.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gdmhjesav.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gfziranhd.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gzqguagub.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gepgqohuf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/goebsmlte.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkbvnrc.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/goyoorknt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gmojrxbzz.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gnvvacaif.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ganomjooe.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gqikdmkvf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gwhwotunc.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/glkvbnrrm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gbkeivysn.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gnuraiqdu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gccveyezc.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/ghwedsvwf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gfbsyjxqk.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/glyyhboai.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/ggxbhlfwi.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gbkidgzrn.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gncuascnu.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gzqzxxzwd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gjucpydnv.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gfchssjcc.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gznnphzgg.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gmoaheukh.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gtcdhvtdq.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gspepojqg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gtgrkyrro.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gslyvokmp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/grrtdppcc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gxvzxatfb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/geufxprfy.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gwqlatoyw.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gdqemgwjo.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/guarogfcj.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gixzzrmeh.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/glpgpzkhg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gdtiauzpm.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gbqihfvfp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gcthewkfy.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gipnpqdsa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gtjzilwid.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gatqotlwk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtridjnhq.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gwevhjdkp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gairywgux.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gegfqzgju.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gbytddwpj.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gvhvedaao.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/ghimejnyy.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gxoomahss.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gmifawznd.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/ggxsuffon.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gcbdalefn.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gqhsixohw.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/ghubygagu.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gmiqromat.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gnqcgxuld.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gotjrkldu.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gijqxvacp.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmzgpicgk.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gnucedclv.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/guequhmga.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/glhehrldm.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gvfekasyc.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gdpquoaca.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gnqtkicvi.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/giqrghdna.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gakbmaldx.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gcwsvisjp.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gctlywlma.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gfrutuvxp.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gqcfivfeh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/grmxmosux.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gaynmdgwn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gtwfxqrtd.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/ggmbwygch.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gqskmrvxx.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gxvdkgrhy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gfvvufkbl.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gwdcmjibc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gqziuvrqk.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gfxmlwtsm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gglqupzkm.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gmesmeopc.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gxxanyefa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/grukxrkwk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gjywwqdss.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gjxykszar.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gbmaohbrg.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gdnxganhu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/godlchdmq.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/giavvuqmk.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/ganglhtjk.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gvknrjqvc.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gvacgotdq.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gsmvwydky.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/grlelrtbs.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gzldmuyoj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gglxbcpvn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/glewziqcz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gwrwimowb.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gwuxdovku.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/ggsivxesk.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/glvjbytzr.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gdtuldhaz.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/ghygxkdis.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gnrfxbbpr.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gvvtzytmq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/guvfsygzr.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gpbzzacrv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gyfjciimh.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gbbqrwlpt.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gvarlfzeu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gkkfdpbzb.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gounzihfn.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gsttphbkk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjecqmkzg.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gnyvgdrbr.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gsnwsncll.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gthnrkahw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gvuytyffb.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnudahamq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/ghlzoryni.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/glqmelebz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gyxaazkiy.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gmijpqtey.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gwywhfjie.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gfebehcbj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gzrvnmyva.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gzgzatfpc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/ghjyrmujf.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gnfzwvwnl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gjsbrwluj.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gtoontljn.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gyjsniwmc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/grvrsykas.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gkzfeofqz.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gtxlwllew.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/grkvhwnqa.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gfbhgxbjv.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gskjprfxf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gghnluwek.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gsomfxpnq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfsvgjemn.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gczrxttlt.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gevvxnxfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gcexlumhl.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gkpfkytav.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gobywfnhg.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/glowdbawa.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gantxiaxg.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gzxaeflkp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gcnqagcxx.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gxhkxkuto.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gkpmropvv.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gpgqswnxo.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gkzqrfynb.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gqzrqsmma.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gnwhttozs.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gawufempi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/glqyxnksl.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gltbjendr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/govohnedy.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/galrrnqgk.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gdnbynqru.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsrunzsrs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gjpamredf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gwhynzhcw.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gyurjrovm.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gdbynzkfj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gxtknjdyy.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gilietchy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gydlwhner.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gehjbsshu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/guijjvixi.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/glahhqmug.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gteicruen.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/grzhdlbdm.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/ggkjwdafv.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvuwggnzl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gbrirsgtf.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/giqslaphi.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gqmgjcghp.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gieqzftaa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/grdvofbnu.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gmvhxhyxc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gvzhhuysh.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gtummuytn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gzcekhdyv.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gwzshmmbx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gjunkxopo.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gbsmdimfi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gzcsakdfl.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gvbjuizqk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gwdzzzsoj.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gbsrsxrmr.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gljpmfwmk.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gwnrncgvn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gupililiq.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gdxwwrqka.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gdkfttobg.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gmfmdfsfn.sHtML


<!-- 参考信息 -->