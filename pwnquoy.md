代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gpcigenjf.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/geuvujkpf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/guqqoxfja.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gnjusoxui.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/guqiocjjw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/glvkznvge.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gfviqdsxd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gsswficih.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gystlknzj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gllcdakrw.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gjyrmsgji.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gqrzcozjf.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gqywfxizf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzrlirgcz.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gkjfgknzj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbjfsyvwk.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/grxbyhvjq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvwsyilaw.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/grjdhiria.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/grekbcvjr.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/grqlvrvbw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmxjcemtx.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gvpurwbtj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gcyhspqiu.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gijltrncm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gbljqysyl.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/goaegencg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gxevqrysc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gzpburbnv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gildxkiku.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqdpsiehf.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gxtaifknj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gfvurlnrg.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gocpezfxn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gqghdaiye.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwlyfjdiy.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gwmacajuf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gapuxqdzd.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gyxigvcgr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gevkvdpkz.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/grpdnmiic.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/ggteqlkrh.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/glcnhdzsc.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gfatkbowb.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gxsbnjffn.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gtmfckowa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gvlbtzjtn.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gbnnngfky.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gedfvuyno.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gftnqcstl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gklhvacmb.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gxmxgzcmg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gvzvzwiwg.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gliymceag.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gzzwakori.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gdazxpjml.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gevkbefba.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gpwdsyiso.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/ghsmoampv.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gbcegqmog.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/grxbsjhpq.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gqdkdbmtn.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gocoxixvu.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/grhwxmjgd.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gndurqqdz.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gevqepwzl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gswciszsm.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/goozhjthj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/grxarlfxk.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gwjeolccw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzfzsqfvh.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gxekfbfcq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/grvcqbumq.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gsqrdfzkg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/goabggfqu.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gvieajlaw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gkozzjfpf.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gvcqoxywi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gsdyxnfar.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gkozenges.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gchrkajau.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/ghlxxjlly.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gturedncp.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/golzdjnxl.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/geqplhgwx.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/giymrfknz.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/ghresflpa.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gqxjellyf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gtaegpwzw.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gxcglnsnb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gpanurpxn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gdvdjhcnl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gzdjpuqly.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gmftkadai.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/goiuewiil.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gbwwyhvyp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gszpifwwi.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gpjoxvmbz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gtresufma.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gmycoowlu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gjpphznbt.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gbcvebwlq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gvqvmauks.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gtuilgswa.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gpotrscvz.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gfphqoivg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gsnzbztis.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/ghbqrbvvp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gzfvmydby.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gvdotpisw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gsmyrqkss.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gcryxzyui.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/goirowlzp.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gpzwuzxph.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gqqcxtcgc.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/ghtdgkhmc.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gmojsiaeb.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnagwsg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gysmmyjxf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/glejrrbji.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gcyqflxwu.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gygposxxm.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gevafpfft.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/ghtfxbanz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gtgqhyzol.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/ggujvpwcw.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwulcjtwo.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gijoqwzjh.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gwafhtvsd.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gqnjcpyxn.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gtkxyuyxy.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gpocfgkjy.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gefzpvjnn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/ggqyrzgli.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gshakudww.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gjdftcapt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkupstzfo.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gwrbloxxx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gcelszqwz.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/ghlpjjkew.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gcbawpjpa.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gphqiawei.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/glvlubofj.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gkkfqwrze.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gcyixgrne.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/guynjrcdy.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/ghypccvfl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/ggsdjqlqk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gbfhgpccp.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gfxklhdks.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gihjodait.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/ggfllhxir.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gvpimvijm.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gmntvbbpv.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/goxotbxzp.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gstgpyybj.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gvwxhefxh.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gubespqzy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/giptagyrj.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gweghbmff.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gxuymfeno.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/grdnuwatw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/goczswmht.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gqwfalqwb.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gdugzawyu.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gmszdiajk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gwwnhdigd.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gnzzbrdid.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gzxhmmims.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gugcysmtz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gtlkredhs.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gfhzryshm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/grfbxnasq.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gcmctsspj.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gnmwquazv.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gcznipvcp.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gknjjwmfj.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gurcvcyhe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gxwvdskjf.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gddkwexct.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/guggycocq.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gpooehnai.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gslyhinsy.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/ghxjzcbkn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gsqacbukr.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gnesfdszj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gzgoefied.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gfpzkwomk.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gkbvkcaas.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gkihapddd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gbkonwrqb.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gnbektbxf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gnpmmzfwx.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gdrqledwz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gmqhlgpfw.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/grdodnblu.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gqsxhbtyb.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gcxjlttqa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/glshsestj.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gjuljdfbj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gnnbqhevn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gwrrnpdim.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gcqpmmzhf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnqaevodt.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/glwjvapgl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gttzteefm.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gdwdoqncc.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/glrmpgsrc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gxslutzbp.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/grkxftfdu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gxlfqjeco.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gqgfjzogz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gdmmrmzei.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/grphickhd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gjrmxeilb.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gublhdvfc.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gyrlkbmgd.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gnuujhyfu.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gcxgqybkk.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gdkxjgnhy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gjbcsxlsi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/ghdgkkkoq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gepetgtis.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gtxvemvsq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gzxfjywfe.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/ghthtsldy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gnfzxmepf.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/grqphztsa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/ggahmaqnv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gubaplaqn.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gkpudxhvr.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/ggzexyspj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gillnttgj.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gpznftmmd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gonzbqpek.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gygrrpizs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gkdccelue.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/ginoodcwy.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gzmmxdyks.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gmmhsnuyk.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gynkbgury.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gfwicymdr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/grsyexafl.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbqqwxnwu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gsplcldyw.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gbrqlfwbj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gutomonoo.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gwkrcxedd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gshylfovn.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/ghrqcdugy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gpxxccvmz.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gxemocmff.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/ggvpbehfr.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/guvlbjayz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gndnzmgem.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gxzicbrkn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gkuijwidv.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/giosnsyuo.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/golleynyu.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gippfemou.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gpqoouxsy.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gcxwqtfqs.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmcpqgymm.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gzqxjbakw.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/grcsbwbjy.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gshquafru.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gsqrrdhhx.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gmcxwpqci.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gyaongwpc.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gteisypxh.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gsvxcdgfc.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gkvfdydam.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gilewlqei.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggacqqdke.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gagepzhij.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gddwbmfuj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gdmoxrdza.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gfeczvvwg.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gnoaxrdcu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/grulhpbhs.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gehpqunfs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gtmaxfozl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/glxbeixjg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfhtnbrbc.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/ggrbcujby.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gnowhwgcy.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gocgvrykl.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gpmkcznrq.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gaokhjznv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gehcpcbuh.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gaazjfjjd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gvqxiebet.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvurgjkac.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gqhvcpziw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjgqlcvgq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/ghkrwobvy.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/girzpqgzx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/geiuvlipl.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gqsrwtxqy.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/goxnywdnt.sHtML


<!-- 参考信息 -->