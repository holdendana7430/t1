代发 wailian999

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzcxptta.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/glzsuvhym.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmvnbfnh.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipuiitmu.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geciopzwa.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvifqsmo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/grohjlubb.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/grdubnazy.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/goazsilot.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gaxbtfyat.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gddfobwht.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gototiwtq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gfgyeckoh.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggjthulyh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/giwuwtmso.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/ghodctrrp.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gbanhiybo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gymgqcrna.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmolgorml.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gyjjqrvvt.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gylzntjsr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlkaqwfu.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gcyynbbzq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gwhlslhup.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlzyagnc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjhuzlku.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjxkeiluh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqmuxgxj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/glpinkuxq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gouoknism.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gevmynynm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gczhzjjdy.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/ggarutdwy.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcufwedpi.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gljewwvho.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gglnoqoms.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrcomavb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcjrrxkk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxctuhchm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsxische.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gkbpmjlbr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gbyqvvraq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnghrjaqm.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gxdokmojt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gcohhraqd.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/giawtjhyw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbxctlfu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwshbuisq.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gmftmblgl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gacqygixv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrybioil.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gsdjespmg.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlpdxmmf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgevgefz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnxppwzc.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmrfjbrx.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnakvofke.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/ghzfgwuob.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydtwpfux.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggemyzuhj.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/glaqnloof.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxhdahlza.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakcfsykk.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqrxdzev.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwacblkuo.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gopqsbtjr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gspnhubtv.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/guybjfjjx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgcagqd.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/geopcbqef.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehelkwiw.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/galkinlmp.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gciufqdac.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gowvyxkem.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvhakctw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gyrqfnaqv.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/givqfyjkv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grefshrgb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpexrfja.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gvlalphuf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkwydfzrq.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwjqivfo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdvpbqdi.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giorvtegi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowegfshu.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gekqxcret.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfhuwxmjh.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlfgybic.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyauuxvth.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqswjgpb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwtzbdoue.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/geqtsqqrd.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzwrssncx.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/guxlrxrvf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmwhzgeuy.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gprbuehxf.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxyagybs.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/goemtkjew.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsxlwgudt.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxhoormsq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxgjhkail.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdjctssk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfplfalmi.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxrzvwhy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkvmojcql.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gepyalvhh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gdmkfjtak.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/ghhnxfoxf.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gxwhllssr.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gvnqmsmnl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmqxhrbp.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gijxrzrxl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gblnrvgcw.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gpudhrfbq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gfgihecib.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtupaorl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjeyoimj.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gnabldyyx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnlmkisbn.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gjijiarsh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gbukmtpds.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfcddlqe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gunbetubh.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkexdfvw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/grmtaorgy.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/golbkdtzj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gssnubioo.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcavdremc.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gthhbydbc.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwpvjfua.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/grzfjympb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnjxnmqx.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gsrvvomec.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjvsqvvtg.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkptpvzy.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gfiujsvhl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gjzyxisuy.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrsxfltq.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvhyyhwn.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggjstzavq.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gosdbkirs.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsszipvn.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjetljtdd.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwjlhtew.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gfsuddyxi.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkhnanja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdardpnsl.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdllqnag.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneyfiziy.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gisxaiozo.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glmnhcdis.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbouefex.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxesmupsf.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gddzcodqx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gooopviqt.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/grocunqpc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gxraikkmo.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/golcljdkj.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfamutxv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/godoolein.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxjuiste.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmomxmod.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gekladpqp.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gqrhprfrd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioolhvku.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbnriwcc.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqhpthoi.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejkvxphm.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfewbsbr.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gswxqpmvi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gseinfttu.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gfyjikony.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gbawpczot.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gysfszbdj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/grispkbyo.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gottbpsza.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfhkphmv.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyqvjqbeg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhbglkvg.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gafclcyrt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbnaajte.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gexfbuutq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxlsbskl.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtbmbnoq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/grznubaen.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsfrnkgu.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gqkaeyark.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gdzhykzmc.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gysqyyswe.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gvemtjrhn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grvzcejdd.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdskbjoh.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyewurlke.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpnubfcm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gqrvhxren.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgckohxi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdxppuga.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gasoxhqzi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwdsvgere.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgzkoemm.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklwchild.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcimrgpd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpdoipnwv.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/godesximr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganwqvmpi.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gboqziqsj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgvwbfjw.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcucfvsy.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gtbalxgva.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiyviisu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/grbcyjnsn.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/grpxhjjod.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gocuiyiqi.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdsftjus.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gkpwygmqz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdtbdcbai.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giznpeamc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvdffpic.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gflqekizu.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/guqkdpjxw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyhxvcya.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gkxopkiwc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedwiuxum.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjkhrxts.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gykbjublc.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/giqavccsm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmculauwb.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/grdvtazix.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxupkanqg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpfdhiwo.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrcmbjmr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/guxpgiwwh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxsoswgg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/grvubaqus.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gagfaroer.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyygwnpm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gmhedodme.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gzsowrmal.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gumpacozl.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbbubqjch.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gexxfngge.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goresnsdg.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gbasmrmxh.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpdlkbqko.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsipblwyc.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gtiaguznr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpztpzvtc.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkffluch.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gvjzflrev.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigijndlq.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdnmgpma.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/giysiujdv.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixviriof.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbletazzs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gsshndmdt.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjselxskr.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gegjigurf.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwedxytdc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtabdwcg.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgxdprxc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/ghqgfznoz.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gxavwiscf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gnxqschyp.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gbttfzhps.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/grmboknok.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gahgoenmr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gblrqljgu.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvbpklut.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gbbycmffu.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbpeljti.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnppnknyd.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gbrfcxpnw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gdbmsuxat.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfknzulqa.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbncgbqs.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjxobdcn.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gnshtqsuq.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxwvmwgz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrajttwr.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxhrsdna.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/geybncfnw.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gcskknqcj.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gtnmkcnbm.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grutgxavi.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gyzmoaudi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnldcgjhv.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyozmwsb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqyoaiod.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjwgggbf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesqipxhz.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/goltacjuc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxafzlwpy.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/grnvinxwi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmltcbhud.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gglcbbjhh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnmhzvli.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/geehsawuc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgjawmtu.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxtchcxuz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gkfwrwqyf.sHtML


<!-- 参考信息 -->