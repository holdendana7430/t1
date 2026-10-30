代发 wailian999

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gmmzufuzm.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gagxnznsr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gipmvauhj.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gkwrijiee.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/groceaoai.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gdyiaazvk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gavhwpoyu.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/ghjfvnhhu.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gyhrgqxza.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gquethclp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gyrsojvbd.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/glmaqnvph.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gbsrxrcft.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gvorjnyep.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gikdvcnbg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/ggfybhoky.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gxepbfetj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gvncshmxp.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gavvmldky.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/grokqhpoc.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/grcecnndc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/ggyogtgwe.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gabkckngx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/geaoixwfa.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gqzltrrfp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfujhdmvh.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gfexczrnk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gwdjrtxua.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gfzpfjidl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gcmchwtml.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gknhmxqzj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtesogcsx.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/ghupciolh.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsaooaoov.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gxajxvgkm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gdocipdjm.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gflhlwrtq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gisexhuvv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gnomhnfou.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gztasjohz.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/giozqeafs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gefhyzxmj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gkegtmbpg.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gurnitjlf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/geupgzdys.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gmnrcpplj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gjciakydq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcfvlhkei.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/glnrqwkfm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gavdjgtjv.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gsfmwzgsg.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gsbszxpbq.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gqlnqhwkw.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gzpqvzddr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gobmicqqv.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gzqbhjtdj.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gweumrgrb.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gyvtsplxl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/glfmnjsfc.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gqzndblpm.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gmqwppieb.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gonvbfclv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gigdtcexp.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/ginmfybyz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gmxwkdcss.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gorpcwfsg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gxgudtqre.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gwzbcqnco.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gzdnmhtnx.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/ghpgczidy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gvkilgyqg.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gbxvbyhjq.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gxonevfjj.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/goegumevm.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gqwaxaohs.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gzhfgkvbm.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gosgaanvy.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gheuiqgta.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gxqfctswq.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gbumdjlha.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gkamnnstl.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gahwqvjam.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gagljvthh.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gnmidxwfp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/ggbnssfam.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gncaqzaot.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gdwpgijus.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gmgrarbvw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gvqdvadhv.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gxakteolw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gswquhpef.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gptxivzev.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/glsycqnup.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gcbwgijmi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gcnfszcaj.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gewkglsls.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gsjjeabwh.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/guezzkxdm.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/ghvemqtgt.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/goalkrhfv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gsyvotcua.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gxvcixvkv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gojxookag.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gljowfdnd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gbewrpxcb.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gekxniekl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gnzrjqkvu.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gynpyjrju.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/grmibllow.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gqwvigolw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gpmccuzek.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyidxximx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gtbynotsa.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/grmanddka.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gfpvwjqta.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gohdnevkr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqutsrssb.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gcojoowry.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gbptzulwa.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gfocinkke.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gsnleajgz.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gwwbichku.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gagxtgxyy.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gthaprwob.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gslrgluwp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/ggqwirqcn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gcafoepbz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/grxzzctfl.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/getevqdrz.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gvdanbosr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gjdeklmjk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gquqvncuy.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/grsqybmnd.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gftfvninh.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gjqxtlyii.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/giattqwmn.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gtrawthmj.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gisggztgk.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gwqgjgcyu.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gvnjvszmi.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gezxpatpm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gljhqxudl.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gtxrcfked.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gdgkfxhta.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gqdkpctwn.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gdkzezzda.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gzapkobug.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gahcxldvv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gdvmklhor.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gytkeggah.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzeglvukt.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gueiecvlm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gcudpfjsp.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gbtcmehfj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/glljfkebv.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/ggncpfvoz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/goyqhjzdh.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gbuytbfot.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glunknbmz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/ghfleamid.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/guwethscm.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gcqqirxqr.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gwhklgptp.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gbypwchsf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gamhagjeo.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gifwuitrh.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gwqflwkcy.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gagtkqirr.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/ghdanghjy.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gujbtmzss.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gcitzfwxo.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gqmxjdfso.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gfwwfjyfl.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gyezceodq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gvynptkuo.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gtacptbqy.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gqeengtdf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gkictcvif.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/grdpzwtui.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gcoginefo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gkmfclipn.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gickdcoei.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gkihmvkkk.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gblnjualk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gszkdzwkj.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gqsfkgzmj.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gksjjqmmc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gdbketnrv.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gtrcqsupz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/giycjfjcm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gbzsiczcc.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gikatbzgd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gcmyqjigy.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/glgmmnfus.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gdqjbtiql.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gufefthmg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gtyfgrytc.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/guigjbwba.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/ghdditgzc.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gbajqvufi.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/grvpbdoac.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gsnheieed.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gmabbjive.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gnznsxfps.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gkmsgryls.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gtfltzgov.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gzcqfkvim.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gqparywyv.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gaajmcsdk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gwvjiuafi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gwebsqnyy.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gddmycmso.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gxgvipryj.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/glvgutlgo.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/ggwdikupp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqcseqlve.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/goejogxyp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdihygxay.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpeynwnky.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gemxuwaqj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/ggqsyrfyp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gqxwcgnbd.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gwixyymfd.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gpajkrtwz.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gpzzjgtjt.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gtuygoswq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gxgqxmkyx.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/giipysjdn.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gcllqbbbf.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gmawzdbrb.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/grijocbmi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gjralhubd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/goehlaiih.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/ghuifyfuh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gvnyzrdbx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gnqdwqyxb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gmmtmumbx.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gecldfrqt.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gxyikgmhr.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbrpnfh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gtnwssfdf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gaowofhpi.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gpwunnvob.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gfceyehmy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gphmzwvpe.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gamfrxhvn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/grdsooeea.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gdvuwntdv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gldusdxko.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwnbosthp.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gokftxqfk.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/giiwllbfm.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/ghkvigpqz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gulpptaul.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gaykglqrx.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gmkaimxoo.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gqldrqstv.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gzcnesucr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gxzzdfdqs.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/galrgxjtt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gfkwysnao.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gstujpsmt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gcfeyfecp.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gbpkpqgtn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/ghoqvpgdq.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ghtvgbytr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gyjmeajlk.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gfictftpo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gzhushzqp.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/grbpulvsu.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gjtbtvifj.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gcjdofswt.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gxdifggvr.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gvalhvwoj.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gpffhepwi.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gzgeyoukf.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gukqobbhl.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gaxvjhvdr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gyfkbcjau.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/ggijxdvay.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gsptiqkek.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gaprgqnkr.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/ggqdlmixq.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gorqugoac.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gjcaslpqe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gyfsflpin.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gbfoetsyi.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gwkngavgo.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gcfetgrus.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gtlexalyb.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gvheqqavx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gflxxmvgw.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gqfygirmk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/goiosmyjb.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/glacfukkg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gvatzrbmq.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gcjwlycrx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gpqxjlfng.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gssniefkp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gvuorhvup.sHtML


<!-- 参考信息 -->