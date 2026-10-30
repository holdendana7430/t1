代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gdersxeuw.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gfykshpap.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjdnyhmrf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/ggclaxbym.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gpkfawjhp.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gocfaffea.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gjbzcpjol.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfyzkgcgt.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gkiibgpma.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjbeuzvkn.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gvgxqqbpm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ggofobtyk.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gkozeksea.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gqwwphkcx.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gbcxvbsho.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gymkrnyeq.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gcxlhgmtq.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gvywwkpea.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gnarbbuaq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gybkvahjh.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gsdhxhcib.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gsvkqcdeq.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gokkiutoj.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gpaiytswq.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gjhenkxjk.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gqypfzzsr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gqxtjxcuj.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gwdbqkcji.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/glaozyjsy.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gdlsljjed.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/ginvijxzq.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gbwapgfwa.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxjevmsdo.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gsotkrwrk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/goiklboyb.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gusdaajyp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gptfptmxi.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/grztrvaho.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/grdotcqyx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/ghhxvdqnb.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gzvdoskhv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gimodvnsf.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gmuhihowo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gqikhavyj.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gpwrlyrqs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/giiuanpdx.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gfulpudut.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/ggmefrzmr.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gvsdntmyh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzuatcxam.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gqkmxxzhj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbnuqdslr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/glfdnewcw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/guthxcbcp.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gsrorxsdc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkrlqotzi.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gsykpjpqj.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gimbvcmkx.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/grclrxpnc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gwmiwmftt.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gptppbntq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gogcqlfoz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gtbpvldqn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gcwturtcg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gdauiqdwc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gcybxviim.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grhfduipg.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gouxsllnb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gmxgwqlpo.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gohesqyte.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gcircuwlz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gftnvcunx.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gaazkunqs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glhyvimzq.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gndeqyabp.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gsqcesjav.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gurvnjrsj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gsdxhvfnw.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gttdrksvg.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gwdkxvvnx.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gsqbtvamd.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gxihhzakb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gglcrrokp.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gkcqtbnqd.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/glofajtbf.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gtdtncrev.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gmsymysph.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gxfgczpqz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/ggpguzrin.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gefuxxwct.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gjehhapcq.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gzkigeyrv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gmvmqgovc.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gowaanlqt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gszxbeatw.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gbgtbwwgn.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gxyperrpf.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/guujapptx.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/greilqulc.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gnquzdxsh.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gzebqoowp.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gmdayjpnc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gzjcgxcbv.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gyszghryn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gnnnvixkg.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gcxzeedjl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gkourbrob.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gpberooah.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gldsutyan.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gzrtiqhwz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gsuwptyhu.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/ghgaaqxbj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gmvpcarqt.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gjohaywta.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gbjnnhizi.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gwuyezebv.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gwslvfmzk.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/geuaahrkj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/ggrsoognt.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/grxwqsvdu.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/goomtgsmk.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gseflacju.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gioqatcrp.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gtxadxpml.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gfnzzknpa.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gzimatrgq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gnltmvhfy.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gpxpvlprd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gqkddjyof.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gtbkzvdxn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gtofhzgzd.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gvihbsqsk.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gmvhcikyz.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gobygckqu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gtystdewp.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gjdrjozgk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gzfuezvzf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gvccrhpaq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gzilgxzio.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/goavykdvm.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/goamlywue.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/grieoeswh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/grtwdufec.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gkzjaebsz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gmumdpxym.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gullpqzld.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/grgephdgz.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gielttkgb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gkpcnwxhg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gukmeuliu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gsosvjlgn.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gsugsadjq.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzbjsju.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gddokkcvb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gzyqqwoai.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/grrctwbwt.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gvxkfxwlx.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gyqmjfwjx.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gpygdvfnt.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/givcfoyme.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gbveetrgm.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gyoyjzkqk.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/ghmosmjfr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gmhvugeae.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gqzespoci.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gvtwqngrc.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gckyrqile.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/ghvtjttfg.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gdmiqfeeu.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/ggesdnfus.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gcnjiavpu.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gqechqfna.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gsnylldar.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gicjwjwbt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gmhjplexl.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gawwaijeq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gpksnmvvl.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gwsdifzxp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gyyzlmevk.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gvocnqiab.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gazqynsll.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gkaysovno.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gbxiudxpi.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gzxgllktf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gwyhquzii.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gbwlfpqyi.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gsvhejoxd.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gfrurtajd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gspraqnrl.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/givsnwynu.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/ggadmyklj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gqeppyzgl.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/ghohxvwjg.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gzzknuzzk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gqyoswlum.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gteokzxkx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gzufzdsdx.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/giaileppo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gxgmpppjy.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gqfpbqlqi.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gysfjqcle.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/ggavqnvvr.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gnokcezkf.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gnfdkbvik.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/giqlkekem.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gybeaoqcn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gxxuaiktk.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gnwumdpbf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gjebwjxyk.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gharwdlup.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gqkgwymlv.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/ghvziqbdf.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gwzboasft.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gsugmhdzw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gviybthqz.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gjmdupfiz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gcsorzxrt.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gptruoylk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/ghszmkewb.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gwgfjbufr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gdeonsevd.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gkwmjjskq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gougfsfvb.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gcilhwzij.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gendxbzco.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gwovwxaqc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/glmcatkpc.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gdxdcqeyw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/grgjqbymc.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gesneerat.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gowscedik.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gstrptbzp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gwsqeeqex.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gflnhpqkk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gsbcodlgk.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gqctkdxpl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gzmdpkifl.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gftizbjcu.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gxelysafy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxcpilequ.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gastioian.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsbnljnve.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gvjpjuslb.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gvswpgyyt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gzkyvtnzx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gbknvgfpa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gjacynxte.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gpelvgvzu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gulifazsu.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gtafwgthc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gfhrgmayt.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gwspjgofv.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/givlcbnvb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gnaolvriy.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gcouxtbye.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gynpyiiyv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gsfmmkvsi.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/geopedmzm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gkmpayemk.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/grllrnppd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gajqjqxbx.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/guzhwlzmp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/grbdvlask.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gvtdpfrth.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gvpwvwoka.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gnecggjrh.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/glikkikis.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gvpideaej.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gccuilweh.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gndpvrqzw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gvnarmgnt.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gicummcpc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/grfhhhcvt.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gsmwvsknh.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gqwheokme.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gxhvdxwos.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gfnavudwz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpxzymuxh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gsxlookns.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gpezaykeo.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gvqmykxfb.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gauohjbgb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gmtfypdxr.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gddyrcsqk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gjtocvums.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gvdosfppr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/ghspkfztw.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/guuckikxg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/ggovunrhy.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gyfbkbknj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gtmfmlrog.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/giyttkvtg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gjxhdnffg.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/geolqmzay.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gzjzphxta.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gbqvmkjnp.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gfkeafclq.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gcxxbvtkv.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gogzmmhmq.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gfjyzfgnj.sHtML


<!-- 参考信息 -->