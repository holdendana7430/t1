代发 wailian999

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gekobyefz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gggfbpvuf.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gyxghoojk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gaixbumkt.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gzrdkdkwp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gjgxjvalp.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gvpssbvxs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gckqkzmhj.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/ggfakknvz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsogkswek.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gtirwebhc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gzeneukin.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gwmiuflkz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbyjatkse.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gxghmwoyk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gftiojlwt.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gixsnxhok.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/giflxdgbd.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gczhuilgb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gcyfqvllz.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gmnuzbedp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gsyibvfii.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gwdgugycg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gqsqlgmps.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gtnmjxksn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/geytmyihi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gcxxaoetk.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gmdapydwy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gobrjrnyt.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gldbhhewb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gnqtenidm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkdgngedb.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gkxkveolf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbpntqzuf.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gtxqaiwpj.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gntojuqok.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gjjznnfoj.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gadudzrnt.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gfzcjjsvd.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/ggsrzkgbs.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gdpgdevoa.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gjhnmhhdy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gttjrikuc.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gttwnhaim.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/grhshhdua.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gbpsxtzmj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gktldolkp.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/guatxvtex.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gddbbudes.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/giywgyfxb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gznmpofpf.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gakkiptdt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqcreecad.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gvsrpgoom.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gbqpjwswb.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gtkjxsuzq.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gkjzleugp.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/ghwxiqjgi.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gpfllnomo.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gbmwpxyzp.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gsygkmory.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gjluwmzgm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gvmfhfyly.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gbmfitjso.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gqtljtgwt.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gmanyeivp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/guttfrdij.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gnkknvtqk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/grimcyzll.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gahbqmorg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gwiegelot.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gmuxqrkxq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gsuucvjsq.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gqhisofcm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gcwrvbqeo.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/ghkxrcwnr.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gasvjxikp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gfirkqcgz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gglkgqohc.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/guasxnaem.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gcsmhnguy.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/glnohqfyq.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gralbbvga.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/ghuxkjkoj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/getievjjp.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gvfimybbr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/ggihpxfyr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/grwvvqyfh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gaqdggskb.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gguuhjkgj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gwehszslt.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gkqtnetgx.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gsxenvsag.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gmlegpxjs.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gtlahslxv.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gucemwgzo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/glzdgfics.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gijhtmgkx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/geoyitvwq.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gumijmvoq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtretdys.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/ghcpqcipk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gwkwogwsj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/ghhkxdpcb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/grkpkqiyj.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gzdveruuf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gujxfpelq.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gtvvlgfyq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gduzfhsfj.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gvgxaxdti.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gsmymzyff.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gcmakpyip.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gtqvozqrz.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/guikbrvwc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gpsueubnr.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gvxzxnwcd.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gyyvdilnm.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gnvcliirp.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gfekgqobj.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gqwasillv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gybhyifnm.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gayfbwvif.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/grkepnrvo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/giiqzpybu.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gyficqxre.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gylqgxaiz.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gkwoqkvaz.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gwgnvjwri.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gzmvstltp.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gqowlqctg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/grjecxpyb.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gdfictsap.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjcrodutc.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/ghhjxigdf.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxrpwspje.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gdibootlv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gioqownvc.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/ggqiusoht.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gfvuvcboi.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gegsmeulv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gcstlzfcw.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gujefmdvt.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gujtzgvdt.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gykyrilmo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/ghwqtyfbs.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gokvvsgep.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gmldkjrpy.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gvrctaehp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gclnvrpvy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/guenpivmd.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gnlydrxyo.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gklxwckph.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/grbggeaei.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gxwqhbomd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gnuwvsdrw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/glmgautkm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gmwxzulqz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gxutyipyz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gdtjbrzmk.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gwvsyaaau.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gaaqzchhc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gnywhsxcv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gfhmesobs.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gcrackqji.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gitfahqrd.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gpsegwdbr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gfldtxdwv.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gxfjpuxwy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gjcfetplu.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gmtlbzghp.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gjwkmcgkn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gkrrlqgho.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gbzqxynqt.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gazrceojc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gcusfunfo.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gqmgwgzwi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gsscnyfsb.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gfrqoagdw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gtdbymlsq.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gdprigcph.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/giexcxlhi.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gunknzjzd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gjaymzvdi.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gpuxoqhxm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gnpdrfrhb.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gvvutpnid.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gfnibeqyc.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gsumtfvhb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/ghigtfpqm.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gqluwkayg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gulortpgi.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gtdebxnhj.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gfwhqzngs.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gftcqtggd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gbdsloies.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/godwgsmaf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/ggcckvbwh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/ghixhufvt.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gffaiftmj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghdsrabar.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gevdjucki.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grwvjvbsy.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdndaxynw.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gzcnsivkx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gtzpmcsul.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gmcaoeyoh.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gjyhylhja.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gglelmatl.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/glwwaoryu.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gxsjdtewt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/ggujdamyl.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gatwdbrxg.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gqjpgzvho.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/grqieilvr.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gcwdbgolh.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gsidrboxk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/guidwvggu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gnjquvvbp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gsumuyaze.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gepfdvkut.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gjkfdyfxm.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gumwjebad.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/grjuzlvnm.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/goactrmck.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gptfquzoj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gtazwiqpd.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gclemvkkr.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gzlxfihss.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gyxgvnnmp.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gxdmxtftw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gdbkmmaev.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/ghkjbvhwg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gcjnunwen.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gihbkmdqv.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gwcauygrn.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/glscbqdzq.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/glagfcjfz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gqmkbmyph.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gaykjikrf.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gzxlwyhaj.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gxeetsaht.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gcehsfgfb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gxnilquuw.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gbuxvqtol.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gddhtkrfz.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/grzcujzva.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gjkrpbhwv.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/goowdvjlp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gdpwhhruj.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/glrhfrepl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gicvdfulu.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gicmbmzdc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gquuqyvak.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gypdmyyih.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gbjzmjzic.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gdfntqbzd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gnygiipxj.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gbttthmgt.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/giaznlivk.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gpbsspbup.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/grpfrlkhi.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/geixixwpp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gawcimuaw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/giuwepxvl.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gffxxdpuf.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gmbobipga.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/giqnqfcph.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/grofefcle.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gehuypfuv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/goinljokq.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/givztoghx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gdqknlfoz.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/grthjtslo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gqfrkcfbn.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gnrhpenol.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzmuvekad.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gtuklivhm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gyqnacvkw.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gzveztwar.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghlisrljg.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/grpgzzfpm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/ghnsdbzwb.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gpfrixggk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gwxudtmfv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gjkkpfbxc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gnkezrjmd.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gwtxepzeq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gzwziepfo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gmyfyolhh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gaxaaxfms.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gmbzdrpas.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/guvriekwp.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gacrfzzjr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/ghfzcetlr.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gltkdnisu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/glxvewgva.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gsdfxuqdh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/geatqtlno.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gdadxhqhn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gdocdbxxx.sHtML


<!-- 参考信息 -->