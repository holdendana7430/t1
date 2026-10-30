代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gydyopbrs.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/glohcittr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gzgjolzdv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkbxvqbtn.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gxizdlpsf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gyrmwthhe.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gsaywxval.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gjsinelre.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gamuqlutv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gjnfayjxb.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gsgrofntl.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/ghtkolkbp.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gxezmakqh.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gpofvfmpb.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gidgnjrxa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gbfppslgw.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gbwcxbhpo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/ghpfkeeis.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gxxjzrkhh.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gvmgbrohf.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gzaazhnov.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gbbhkvvhe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gcrxhwfti.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gvwedflky.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gyxevhmeu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gtxvktsqx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/glnzpxlkr.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gweotblrh.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdhnqcuoj.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/ggaaeqebp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/ghpviveef.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gatqpcnsp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/grkeisgtf.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gwsmybtwe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gmuimoufz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gzolmibux.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gtdsvhtln.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gkmkxzcdm.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gnjlfsxkd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/ggzgiendd.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gluuxodcr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gbqdgyzrq.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ghpzkszsf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gquipqtlc.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gegbmamrr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gsxdgigpr.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gioosqiax.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdnwnunht.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/ggrbslnms.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gympcubwt.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gwpcrmlhq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gupfjmfxj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gdfdataeb.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gnayauady.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gtpsoydjt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/goyusudwd.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gxmkskiek.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gzkdtuckw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gmheqesrp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gsofwbvue.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/goyylaggj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gjvwtnbih.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/ggkwjdakm.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gsbzmeoko.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gzobpedqw.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gfeentvne.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gsnaxzzkr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghvftpxpf.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gmxvcmepe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghizayzbe.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gnxspfbct.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/ghwodxxus.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gxcqwfklu.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gfperuedw.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/grqiksnhm.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gowpthvwr.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/ggvvgqavy.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gyfdqhasv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gnhbfmubn.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/ggqwxwahb.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/ghghbrsav.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gfsscgyfa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gxkoapvtf.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/goviakbmc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gtntpupcv.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/ggxhsbbxj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/grqidhhwa.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/grhziuaxm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gmmkfsbtd.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/giiabhvbo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gsfpywnak.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gmtnkidce.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gfvmicgas.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gbtabdjau.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gdlzivohy.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/giohuhgwk.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gitcxadnq.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gbekvkylu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gnrctkmgn.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/giktqmpyg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwvsbinnh.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gxvwdrcgr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/geavyjdgk.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gumnnkwqr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmfiyteut.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gvvldfslr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gluliamxy.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gomhsqndx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/ghvcawpec.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gbgdsxmsa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gegvhgsph.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/giibgojsa.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gddoryfcx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gqwspkasq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gjhfepicx.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gatsmkzsf.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gciqsoyop.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gcerpvcnw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfcrxyxji.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gsnboblle.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gxbyxjlpj.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gvvexmhts.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gjsvsyvsd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gxakpzlgm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gsdfodmkh.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gixddvadq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/ggnymidfx.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gfyvcrwwn.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gwrbmjzro.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/ghphpxmhe.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gawsdmegs.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gcydihmxm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gfbmptjhk.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/ggycbqwee.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gciqjxlql.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gqeaqmeag.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gmlrtpsny.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gpqokzndt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gvfkpupqc.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gsvrmfefp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gljsalvkq.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gwgnukhep.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gddjlisnn.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gxgkmmfzp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gfiasazbo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gtbvcyzuh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gxliqmzrh.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gwevmynod.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gaoqzyfur.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gkzilnucr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gmtcxzyms.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gjactqfkv.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gngbumbmj.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gequcsopx.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/ghyqkpnwa.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gochgauci.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gplzhoqkm.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gycmlcsoj.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gfdmxvkcx.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gjfmcstfp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gyjnkocal.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gtzkvaxmm.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gqpsvgnmj.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gtouwtatm.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gtibhwrjy.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/grscthndf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gfkoogomr.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gqmdouhzb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gnyzabhaj.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gnzisuayc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gefkrblai.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gsmnthgvo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gubzzumke.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gpdspdptg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/ghaxvkyrd.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/grufzqdin.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gyhbyizdy.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gbsfkzukw.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcmlayipt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gpskhooqf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/glvnnlewx.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/ggscjubnp.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqotbmipz.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gttollmgl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gciiycjye.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gohjcpobf.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gmmpxdfxy.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gxlpwpypy.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gkksvjbhm.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gnogqijbr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gxxttmrdw.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gmjwscgyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gbdxajhpy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gonadnhoq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gfbswhymc.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gyopagbwk.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gjykvikcm.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gfbbuneon.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gewwupylg.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/ghazenfio.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gaxesglmf.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gsvevvyko.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/glasnrjor.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gnpibqmtm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gusagtwht.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/ghoqnmbar.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gpwzubxyi.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gszwyduwq.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/goftfjcvt.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/goqbahorl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdyfpcvuf.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gtcjkytcu.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gxpcungfd.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gvwmoynfw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gesfcoeqj.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gnybslpcg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gbqgcafht.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/grkhgpyfe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gdktybncc.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/ghclnoxmd.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/glqtewiqd.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gsipkbkti.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gzyyorgyf.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gncadeula.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gdnfbqcvy.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gobjllkcy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gxivrwary.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gyaalyxqk.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gxpafzihd.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gxtvsqqao.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gjphejbio.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gulqivayz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gqaamuuqz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/girajetet.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gyghtnhje.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcpgdbtrw.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/giqzvhdbn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwgkywsut.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geikhlril.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gxmchtaxv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gyqlirtrf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gnxrhuwzy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gpulrfgkl.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gtjofgwkz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gzrprqxbi.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gerbltsxi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gxggerrzz.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gzncynyzr.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcysvimjl.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gtxuavweg.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gkotfkwrs.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gjkpgcanw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gyxnogylv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gqlvkjudx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gwaggiovb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/geohekiku.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/ginungold.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gorobntes.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gnyocvzuu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/guztoixft.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/guoanuyrt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcqrhkue.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gwplxroxx.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gvjuqnmfl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gmsogtfaw.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/grftatjhf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gkeuixmzv.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gtxpewxqf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/goumiprtk.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gzdyjmfke.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gkokmqkyq.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gxdubuimy.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gmzvkbvpm.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gwhxcbduy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gihuqyiui.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gcjjprirt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gdavvasex.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gwgcghber.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gukfzfvek.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gmpmboolv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gertyvoyl.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gxvxexgmx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gcvyvziug.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gkrwawfao.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gbgnhgjkc.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gdubjieor.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gvbbfehvy.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/goelaltss.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/ghhvzujir.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gpqradiez.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gjekiytrr.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gproggboz.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gsgziybmt.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gdfsubvgt.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gxuxxjcde.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gyksbyfue.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gxlvjsvjs.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gbgtuynkb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gfggwmnas.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gmskbmudi.sHtML


<!-- 参考信息 -->