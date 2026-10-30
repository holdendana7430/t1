代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gszmprvgg.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gcpddatrz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmbszypod.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gitugxxau.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gvijcxckh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gbzqrmrll.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gnlmgpbxa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gqmxfyfza.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/glusmthaf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/glmjjavnw.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gajdjmfks.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gwjsblodk.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gggysykpu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkaeghcxc.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gqxzfynwl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggecqivxi.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gytagfbaf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqakfmrsm.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gfytuxvox.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbqdwacky.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gvnhjybou.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/ghqsqfvep.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gunfgpqrp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gpukrhyqs.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gzpmeukug.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/giwacodqr.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/ghybvrfit.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gaxsmntjz.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gpzydmois.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/ghkpmziol.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/grpdtrucp.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gansqhstb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gkqeeuvxt.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gizrfcayi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gvschasjv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geuncqlwt.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gjhxnnkdn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvgadtihj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/ggveocdkg.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gfqepcpjf.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gdvwarkni.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gutmeqxbu.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gyywyjkbj.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gkqlxtpry.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gogucocjt.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gvteawgdd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gkthmuwun.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gsetitrie.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/grmoyucke.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gixjrkqpd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gyhxyxkvr.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gzhbbjufs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/ghgrxdsyl.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gkbgdofyf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gwmjmbhaw.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gqhulafkh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gfyonuyhq.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/geifvaari.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gaubteeax.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gujqcxugs.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/guagxexsl.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gbrgrpwul.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gpcmgawrj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gltpqhetl.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/goevvfpyu.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gnqlqguyf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gbrxqmmcg.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/guxrcueuk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gsdfharvj.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/ganxeuzxs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gboeqlbit.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/geyiwkyya.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/geirnhbrz.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gratpnixs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gewjtzmpz.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/guipywpij.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gxhlgxvcy.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gubsiztwl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gvrbuarin.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gdmbemlpr.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/geyajcopg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gzntecqag.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gmihivjym.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gmxpwrknk.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gvlbmkrtv.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gfluobpur.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gdsgprqab.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gwdqaxusw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/ggujjsugc.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/grxdswphr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gmhdyzizq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gguiotapa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gfdzcddas.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/glrheitqu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/ghwmmrmvm.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gkqelcige.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gbsnyhykp.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gngdwgjuj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gvekmezkd.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gnoitcdau.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gzsfrcgiy.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gcsmptdeg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gjsglmsgs.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/glnstzkev.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/griagsxfi.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/glpsucxvd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gidgjwpwx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gixepacgw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gnbshbusp.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gceasttwm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/glziipyit.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/ggozxzahx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/glwfnvxrz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gwsgrxabz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gcwpassjc.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gkmjdbegd.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/glnvivdya.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gplvsfifr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gzwjnxmla.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gtupmsogt.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gncnfnpql.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gmtouonyx.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gyeqjexey.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/geqtbvkxv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gdahsbuvm.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/grqabyvld.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqhdxfpym.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/garrhvxil.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/ggqnppfip.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gmbqzuowk.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/giovdvxii.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gyralqwuy.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gypjuqibw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gdyllouxe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gqnarxmku.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gqnmxrmsy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gafqtyccl.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gghskcspw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gpvpjthee.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gzozvqpzx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gnpmyoiit.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/goxrynxfs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gqvrojqya.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gwjgqewnn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gcwjuvaeh.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gujsnoncr.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gnlncopcr.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gyoxnvybi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gjwdoebha.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gcscksbbd.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gyikpqojs.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/giigsdkel.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gzuifvkit.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gjqjlhbad.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gvztznkxc.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gjcnhfmcj.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gdwpjnltl.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gevucsvkp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gtxemncvy.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gqsyxiixp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/ggnkzwudh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gdxzjnoyg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gncbwvepp.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gtmekjhqc.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/ghgxwmgey.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gcpunyayl.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gwwonymla.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gumvdaynq.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gjhaoesar.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gstdiwgfy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gkwfcgpde.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gnlgubjxb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gzxngenno.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gllfwivvw.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gohmfzwxl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gnwounjwb.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/ghsoxmceh.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gsjphflpw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gglmhfuhi.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gbnfrcdbi.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gjmzdcopw.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gnstpapex.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gjnhgzymv.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gkgehsfwm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/ggwnqrpyz.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gyfnufmti.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gvfzxdvei.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gcapntbqk.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gdmxlagae.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gtskspgxn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gwwmssocl.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/godtnshug.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gsixkyxfb.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gmnylzfju.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gnjpbieoy.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gdntpwzly.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/grjwwsvjx.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gfswmthsx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/glskxngel.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gdbcubmjw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gcbypkbte.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gjrhfjrnx.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gausblwah.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjvcorppg.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/godrejabu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gspasappm.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghwtltsju.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gghhvfcxe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gvjgetzye.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gmqkiloyq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gdpzjklht.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/ggphnkdfd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gxyugzabb.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gfhompkjo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gucqmgmkw.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gggelgknf.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gdawtzwyw.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gsjgldccr.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gwaktjssc.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gkfvnbcem.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gvldmopnh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gbaptnrzc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/grubckfxi.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gbijrtymo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gswkvovjc.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gmvpxhzrq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gtvgowfqi.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gxhnpsdcs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/grppvzuii.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gewooxcfy.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gkjcvmgvl.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/garjdeseg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gavnmqcof.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/ghatidvsr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gkreqexbx.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gdewofqgk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gzduowuxt.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gzzjnviqb.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gbjjjcayc.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gblmljeeb.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/ggnyjdhuq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gwnlkyqae.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/ggavjcebb.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/guipdudjd.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gdljoezyf.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gngvhqvvj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/giutmspoc.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/glpuyreht.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/guuwvthki.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gvgwzicyk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gqvugcfkm.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gywryiofm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gnpbofcwd.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/grwvnljuq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gopnwmykh.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/guzlvruoe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/glmfrsxul.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gqvzrupej.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gkxbqamlt.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gwyujnjri.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/ghmqtrarg.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gtoifdoid.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grncckjve.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gqylvqtlw.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gctfedmhu.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gfnsfbmpe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gcuxulcal.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gdtyqcuns.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gqphemtef.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/ghralerxh.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gafbsbtyr.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gmhfspwve.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gzzkechbj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gxwmstfxy.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gxkezfdkn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gicjxeyzn.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/guqiqbzwl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gqezxjhes.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/ghxikjswu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gccdowcga.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gggnkgbya.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gkvzteilr.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gcvssqihy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/glonhxwez.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gsalfgrgo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gyrgphbnp.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/grzokltoo.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gqrmlmkjn.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gqfntevnl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gyearfekk.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gcdaluesd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gexvlwmbp.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gjjxtmila.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gommlqjvw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/glyrovnbl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/ggydxtcxv.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gjqonewys.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/grhglmqgq.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gmojhuutc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/guzvwkmvh.sHtML


<!-- 参考信息 -->