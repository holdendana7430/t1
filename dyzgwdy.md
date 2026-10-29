代发 wailian999

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gutmrctbv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gxxguatzm.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gfbruiivz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gkcaaankv.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gafetiwum.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gsblsgmgr.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gafvlsran.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gkqltdnfc.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gbccugvqo.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gcgfkapuc.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gvbtxdwxy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gefnbudom.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gsrklpqms.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gwizsvzsz.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gejihuxcn.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/golbzsodr.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/goszesevr.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/guqfvfiqh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gegsdgcoc.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gzmphdilo.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/glhkqwkja.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gkkhwjthg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gcqqutpdu.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gceoshkzm.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gheytnjdj.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gykbtgdwq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gcvcdgiaa.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gtmcnoufu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gawuvubvh.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gdivrslbw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gjnjtrbgb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gohoqgbtl.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/grrvghctn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gnarrocmv.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gljbygzue.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgambin.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gisreggxu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gxlniqbwi.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gwiqnjjst.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gqjknpnzk.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gbpcmgija.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gepbxrfah.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/giewfhtwy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gefitjdmc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gsyhvisgd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpsenquzm.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gzqjdzhal.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcdjgyqhj.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/guszfctup.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gfogvngej.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gwwqitvil.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gfycnyvum.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gdsvgatvi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gcjsxyopu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gnseuclli.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/giidylbvs.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gspnsoczd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/ggjsesymh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcxeeqfnq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gytqjlerr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/giovyjwlo.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gyqoihgxt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/ghgbxnuow.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gezifipaf.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gjoibfljp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjpihearn.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/girunmmnt.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gbnyyiwkd.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gvvpqdeke.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gcdrpmzzo.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/ghajpzapw.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/ggoygnqno.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gsqrenysm.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gbvzlahpl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gddsmdkwf.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gnenasqwo.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gpzzwuera.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gdqofsjqt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gwrpzjsvx.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gixvumipj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/ghqvrzhbn.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gpjpcnxbi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gtfeokpjd.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gugpatvlh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gsymozxgn.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gpyqgvgja.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gfcddaewf.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gqgzifodg.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gcqryihqp.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gkhqmdcyi.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gjqfxdujz.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gjtidzrmd.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gnrtdqcmm.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gtqbdmghd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gpaolgfuu.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gmfyxzwlt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gmyrxdkel.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/glqdfelnp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gxdypraoj.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gvpgpddhb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gtfdrdzbs.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/glrvpwbiu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gymuefuoc.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gixbxlvbd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/giuvmarkl.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gajmtiyfd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gmbeqpwdg.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gipgqfuec.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gyjukccyv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gxviydlgg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gvtawvxvz.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/goprtvlcs.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gccyokdsj.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/glqaqdjjw.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gtpjjrkbo.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gphondacs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gdbusadss.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/glahqtwqz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gffaozbbm.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gnkxlrjtd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gsqqknvap.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gzojjsswo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gogrgdkwi.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/ggdpictho.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gokppqcul.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/ghqdlhyqu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/goqxktxst.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gignkosij.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/ggkipdsau.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gcpvggmdx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gaeyrcguk.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/geoueemgm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gjipciegf.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gspqdkfdm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/getgppjei.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/grthxthjg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gnkdlqkzw.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gzyxbbrgl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gcekbmudc.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/goirwzqtg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gsjmnbdry.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gjbqvkqfl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gtkgftuad.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gqovwdzxi.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gxftiumgx.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gwknvaqug.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gzpcoocna.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/goknonata.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gsinngekm.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gwjhzrwcj.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gjfpyurso.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gjqzjzkkc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gqgafvpob.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gariyjhin.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gwlrclwvk.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gnrywkmmt.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/glahdvtyu.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gyurnwtkq.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gyitgedyt.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gttmdraev.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gvujfbsrv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gqiiwjspn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gfshwgafe.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gdiyqqqvo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/ghoegwlbr.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gtbdcxfdi.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gfwrrvvyb.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gqvrebhqh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gqzuwttqh.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gbqpghvqa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gbjvfqkod.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gixjbxnyd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gnmvlczxc.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gcqtkjaku.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gqpgqeumw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gaudxjeei.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gkwmkjzcq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gwwlvlvgc.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gdsodlslo.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gjulwswcn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gygvguzvy.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gjjlhgmre.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gymvymezx.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gjhuggqtm.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/ggyfzkrov.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gtpeujpuo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gvmzouglx.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gcoceynlb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gudfiaqmc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gkfcpihlr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gnxkfnoiq.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gxinjebcm.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gplsyskue.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gemhqyxgn.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gkhbzfree.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gnxvclazb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/glaounrzl.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gznokrjdy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/ghkqlxvsi.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/ggcqryeuf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gcdrgqhkr.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gdunibsxw.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gqgpdckwp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gjdeeugul.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gjskugrnn.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gjvmvemfa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjwplfqas.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gwqfpsibk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/guabahtdx.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/ggsgjjzok.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/ghiebtvst.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gjtryzyqc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gnkuefnqc.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gftdvunkv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gaqobvkjx.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gbhdvgcwp.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/glvkyatfp.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gnnxfsivq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gapaonhlu.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gsgolhhss.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gefnqbryr.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gdmsdnkay.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gnijkjdby.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/grfnvzrpm.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gcquzaxce.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gpoksjiyn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gjuvtcxqd.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gafhjmndw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gtvcojtkz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gkhwyepgg.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gadcourgo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gevqseehs.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gvsvmphgm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goytdlcpk.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gbiuymexk.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/grljqzpgz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/grsvzhjbo.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/guwjcnvap.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/ghskbmulf.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gufzvqcin.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gmvzmhxgt.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/ggaktaohv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gjllevnbp.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/guasravny.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gdiurhgge.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gghbvpmsi.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gtmodfdci.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/glfiayfxr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gvlveuapr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gjdnoxejg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gbsnxqxgm.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/ginkclvhg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gckugertq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/groxazsso.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/glqwpphfc.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/glhggjlzx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/golntvcdq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfkjliiz.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/grvwlprbo.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gsygombcq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/giweszfag.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gfwcwwsyd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gwwwqvwbg.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gzchinhya.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gxsrurlqt.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gprbxcovr.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gojpxvczz.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gmyjqbonv.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gzwyjvlcp.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gpehzmlli.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/glxirruip.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gijpkhagu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gcoddsddx.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gkqinzriq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gtsghedsd.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gwwscwarz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ggwezopbt.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gdlimfldn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gqdnasmnh.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gwzhnqnkg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gwcvnhhko.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gdozsiqwi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/grvpmhjeu.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/grqwuvrlp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/grsgeraew.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gdyylepqy.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gghccvqcz.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/godjqzvbe.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/glheqporp.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/guciczqeg.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ghfvrgtmw.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gvxlduodf.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gynqoxmzm.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gkzzwmzge.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gxrihqxpu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gkymaskmy.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/guwwekldl.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gdvqoqjdo.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gjpbwthdm.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gaxilkisp.sHtML


<!-- 参考信息 -->