代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfrhpkyvr.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gqqzhrrls.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gzincbycj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdtsmxvdn.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/glplwqhkw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gknbulnlm.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gjreawsex.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/grjmsqupg.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/ghrfqfmqv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gokesmpel.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gwjzcqtvb.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gxohqujvm.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gtbyytehq.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gmxutwwov.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gqxpunljr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gnqzvmact.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/geyxwrbyd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gfnjjusfj.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gyofeiuoc.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/giifvwhdz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gwbkiknhj.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gdhtzjdkb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/ganwzdzok.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/guydoespo.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gifaocnct.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gqrgluxwh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gwgcewosr.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/glndujbqw.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gndpebzur.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gbhsxobvv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gbeevfvfc.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gyegsjwul.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gpqphysvw.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gochqoqmb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmgskwyca.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gqdubynju.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gprcfupuk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gmliypill.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/guyeshkiy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gcjjycfik.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gwilprrux.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/ganfkxspf.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gomdfxxgn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/ghymwahux.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/glsylirpu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxjrzmimi.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gdivarxmt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmtqkvita.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzxwoawdn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/glzjbpqgc.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/grozwxcad.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gceexzxln.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/glsxkcdwj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glfnagnxf.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gzsdbpjah.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gmepzamjh.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gdlceuivr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gmgjqvfil.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/geildwbkr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gjwrcdnpd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gtupylrey.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gotnyrsqa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gncsiymuy.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gclwpwyid.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gbtcqfjfq.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gzycxyqdv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gbuupzktk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqphdbszc.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gwvdwlews.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbcvfjbxw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/geglnuhvz.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gvyskgdoy.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gsoepellu.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gjxhctalt.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gnxruyqwg.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gmlpxzitf.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/glptensyy.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gtggqljla.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gvjpvczqz.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gtjzeespk.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gvaxfpwrg.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/grnkciuxf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gchemcsar.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gtzzgzxor.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gyxxtsdpw.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gaqjlivqs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gbuhrmdkp.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gefksogcr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/ghlpwaxhk.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gdfbmqbir.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gpbqelxzb.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gefthnxpl.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gbocjaywk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gtsmrwcvh.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gsvvpugfp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gkefdvxtw.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gczqgwyjr.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gojojtfyr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gtkhftyxe.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gxjictncs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gpwvoqtkf.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gkynvaubi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gjctxlwqg.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gtdkijqae.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gozegyyvu.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/glmmzvbxj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gughrsnep.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gfzyrugzo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gldoghidu.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gyyowuybv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbnshdjvn.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gyjucqgji.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gzmhflihs.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/ghwezzlgo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/glvzxwims.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gmlvfjvrk.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gxtlxwxyt.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gsdtzlvlv.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gzvbxyqja.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gmofmgepi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/grmuucrwv.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gbmwgqkju.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gtwktjxxx.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gmldqlkyy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gpomuepdq.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gjpxqlysw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gqbsxyoof.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gsrtgcpme.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gtquljkjr.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gowbelhot.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gefmoxerz.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gafgrnaxd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gytcngptp.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gyghqfvxj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gwvgsitgd.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gbjtgzddj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gjyvfusqt.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/ggnhrhmnr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gwvqntwjm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gbphzvduc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gdwmjftnf.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gfwijzcnx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gdaeyaqsv.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gxpflmrlx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gyustvjsp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/ghwknsqxn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gczbcpalp.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gkdkdemzh.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/glcnixzya.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gplmumuto.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/giksijrvp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gmhqbcxth.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/ggzzzdpda.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gufpbubtl.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gdcojqffx.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gxkakaodr.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/ghmhyuqtr.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gtbvoylgu.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/grgfbfcez.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gaodbcavn.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gkzxdbxxz.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/ghybruufp.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gexnhthmm.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gfjvujueq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gfrftwhlw.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gqhmgaiqa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gthvgfxpb.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gnupsmslc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gvlkcdnrg.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gkrdalbzi.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gnoeboxbd.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gzacxmtnx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gblpjvgqr.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gugyvwlax.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gelcnibhb.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/garoodwsz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gpincviqz.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/glgtucsaf.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gyarxgqoq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gnbkaihjd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/ghnabpkra.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gmbmnajtl.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gpvnkuobs.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gbwebouzg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gvixfejvp.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gtjxrwzad.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gjnhkfhaj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/grhyroufh.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gkmansjgj.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gysslslsx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/ggpdhfqxi.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gwzhgvnbk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/grtagyhhe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/grrfdelce.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gjvfkezwo.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/ghcfkgsua.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/ggrkwmqfv.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gtjcuqfjf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gdtgebcas.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gdeqmhsvt.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/glweirtqq.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gctywdqlk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gwpcwvkyw.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gisoxgqeu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gxgaipcbk.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gvwqljksy.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/giddsxhyi.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gmkshrdkw.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gxcfrwgdg.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gbyqzjrlf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gnqfimvkv.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gncpqoigw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/ghytidylv.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/ggmkkvoty.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gcjmdllpp.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/grgmqjpld.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gcllbewte.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gzokggqhh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gtpkbgiou.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/ggejugswx.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/geuajjczv.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/glowadbih.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gptugvnhl.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gqlwjdaas.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gkoylfsqt.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gqxukbkcc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gpwnsnbiq.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/giugwhrjm.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gvhcmmdvb.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gnhmjakbe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gztgjnabi.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gqanovnkm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/glyilvcax.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gdjibxlly.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gxnrtrjyd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gipodzoaa.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gezczptqo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gncnpwyex.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkumvgdnc.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gnagmkhjj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpxqvnbb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gkqwonruz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gfinfwtbj.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gtobwpiqa.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gciqrrubs.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/ggjcmrqnh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/giktszerz.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/guputhkkq.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gkdalttub.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gjefxfovc.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gaaeotoyr.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gkwbprdia.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gnbdatnsh.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/ghmzbpbfh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/ghhhmusvq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gszmpkjhl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gxbzukhqk.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gmjbbhipm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gndoglfbi.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwbpmstck.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gzylevghw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/grsuyhziz.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gyblbkvei.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gthzxvwsi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gwjxgceru.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gppcgoiik.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gcbtbloxy.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gzpakcpol.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gszrhnpir.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gratjnwnm.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gablthhzn.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gywjhobfq.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gqneqgolt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gsbkxrwjw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gvhcctnlo.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gklonkale.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/goqkmkojf.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/ghbcurdlf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gkspbicly.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gnlqtisdz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gameqvuat.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/ggzcywujs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gjwtsjoig.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gmrrafyrn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gkhtcmeyv.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gpfazjcyz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gxooqrnwy.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gtmjojiec.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/glntntpsr.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gphprqxso.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gvoyjgout.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gfwxmvzwo.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gxemdnmjz.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gnkgolnht.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gxlmpqqmd.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gzlposnje.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gjvcljkee.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gjkxpuudn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/ggvvvzytv.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gcluemqwf.sHtML


<!-- 参考信息 -->