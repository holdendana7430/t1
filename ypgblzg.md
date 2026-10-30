代发 wailian999

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gpimtkaxf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrmsaxll.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxsoxuau.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/guoscmzcm.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyulkuut.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwxxpmgw.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/glysocxdq.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gtclatlaj.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gcyylosci.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgwtaxld.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gvqikczwj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvtwdygu.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gxqsbizqm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/guroirdfz.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/ggavuwkmr.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbozhjaf.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqlnmliv.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/girckgvqr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guenelicn.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/glipbtyiz.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gptvsmqkb.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gxjrywftx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gfslufdsr.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnwicjfj.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ganzgihxm.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygiahvmc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucmczhju.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/guowpdegj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gwqajrikm.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gibsvmgol.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwztntlc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/guvxvnaaw.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/garxulrod.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gkmipuuho.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/guikjnowb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gkzxhddgd.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/grwavcrhm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/guifllzkr.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gbbtkpfso.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gjqcifsqt.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevpamylb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyjcfgcv.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwxshvca.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxxkwlgmp.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdodtrngb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzeqkcrdd.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gmkpxkcjn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaybiuxq.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumufyhwg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbmjryyx.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbowyuag.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmscldlky.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gthtyajte.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqkjagjl.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gtrzbgbnq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gqxqehngk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/glzqwlmqm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gchozdyqk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzepszvux.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gmdoeonem.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqynjmlqz.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzaukbde.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkureztgf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grziuyrho.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gywyevdpo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfcbfogp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdszhvju.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/ggccsbasg.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gzmjpwgux.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxquowxf.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzkppgmb.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvclaglx.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gellmzkjl.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gnvdlqbuf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/grhjyvykd.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gwfuujghg.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzswyuss.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/goprjrcsm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtswojnyd.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/grjcmxdze.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gehyaxaob.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvjbkbaf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvdvdfxf.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupoqgnzu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbprbuum.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gzdgkxhaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtynnkpy.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfootuoya.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/grkuarddj.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqapiyinb.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/grgwetukc.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepftnael.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtelmuvh.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmauoocgl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwbyvsun.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gpaskciil.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gogubsfam.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/geyixnleq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxasbabgi.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqjsdacdh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnwxoyilu.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gejksenem.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnypxnlnz.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gcvqqowtf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoafnqfr.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyekbqga.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqcvgzpxm.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuodoihg.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsexliab.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoerfcsu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwigtsheg.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/govxlxvin.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboqwyhyy.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkozywfqv.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gajlhxcab.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/godqjjsbc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggycjtzfn.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gskbxlimy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfrpglvr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhgvlufa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzqqtqqvr.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawwiaffq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gdnesllxt.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gsokmosaz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhswhtrg.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoxcjged.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gfcuohopm.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygpudhcn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/geewfogzn.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gzmnaqpwt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfikxehbo.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gajncextv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gllfcnibe.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gcagqbask.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxajvfbuw.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/goetzggbw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gaxwhsvnl.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gqspwemkj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitxxpfda.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gmvuetryq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gkegafgyk.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxlkeilo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmulnsqde.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzewfacgq.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvjuwdjf.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gqnruzxdl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gretylcpd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gheaszaxf.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ghvnknmvw.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/grkupyrnf.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlkynvxj.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gyyftsjca.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhaxwuio.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmdcbqoh.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gejekolie.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gaoefrekx.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gtvljvjrc.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxopvllq.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gnfaaweym.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gszorjrxx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvjfmnyd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gziculkat.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/glcqladwr.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gaykqsdxc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbapujfx.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gnevspguj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gplpukraf.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/glghwjeic.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqmolhvw.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/ggudpkgvo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcnwwsxnv.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gtzcldoon.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbnrormc.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gmwptsacx.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbplbeamc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/glxsbnfyu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gcytycjbt.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjiwryhw.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gryochptd.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gdvrspnpu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gqklmgmlp.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gewuiukks.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gpofnecqs.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gegmkcatj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvrfavtb.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrzcwhpx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsztxvuvg.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvhlrcyd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gieknoroa.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gszmhcjei.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gpwghvjvu.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gsbdbdojr.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvhdbnno.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gflfiwkjx.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gmnaowzhj.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gniyejbra.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gclgbdzxz.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtexshwt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuzinvke.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpgjxpfm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/germtunji.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gcsfriixu.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gnceaqyoo.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfvqzipk.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteahqkgl.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscaqoocc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpsfrktx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijklnwgg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gljfkxteg.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuwgcjvi.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjygnvwm.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gekfwrvfb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/guobagfys.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/goarnhlrx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gamvxxmhc.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gnffygkhv.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuwfgrie.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkobnobpt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsllqgkt.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gstldaqrj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gofqdiimg.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbrwyqohw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/goqdroymu.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gfmhlmlju.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/ggatqxttl.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gxlabtezu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfecfjroe.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gqsbiljkk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gidlskgby.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getfwkpru.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gddwmywpi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gitrutmuj.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gavysttgu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvwladysg.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgzcahzm.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/goqewapap.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcixfmdey.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/ghsdbhndn.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gyxfesaee.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gwwftxnof.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/givhblpnh.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtrdsraq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gktnvljqx.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gkdjwejea.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcwzlzfu.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/goqbiwtru.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmqpzvwg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/glnzldrqq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gzyofesbr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gmisgonzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gptoqnvmv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gkucpcvqo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gdbtmiize.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gnniqqjmr.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gjlkuuyxh.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnmveqru.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/goahyrrvc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gedkodvha.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/glmtlvfeq.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gawuutzrb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlcdvymz.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmobwolf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqktammca.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbizbjusr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gzogkncba.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggisaalyk.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gkthdsstz.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgywhqfd.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhgzyoou.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gobydgjxc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gysvjbfaw.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gftdngosl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlrwlumo.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhkyvggs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gphnusgkq.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpyezypb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gldfftsqr.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhxdheqp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gapaskiba.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gaezrpbyt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/glmjxyipl.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gmcliaffi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gjdmkfrmm.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gejzujudb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcbyhvrh.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/glbunvwsz.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gtjkiafzl.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gcjrnbeag.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwapiqcnm.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcmrmwcb.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gumqkynhn.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gygpqbuml.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghevtaqpw.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvbapbgrk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gciuncioe.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjebnfrb.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gibulmfpz.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gizjqxlwa.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gdasudyen.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdaoivmij.sHtML


<!-- 参考信息 -->