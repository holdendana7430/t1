代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gwcmqzahh.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gimqxgpyh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grxagbdof.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gmezjltlg.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gopjksktf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/glhgwxjuj.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gzzapvyai.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gwxqtatll.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gbsggbtgp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gbewrntgv.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gqdyjiugc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gxvbsgxko.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gpupscgpr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gexlvhxlm.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gmuorarca.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glawvlfps.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gjfyoileb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gomkynjdz.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/goakkzpog.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gaolrtqic.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/goifeuona.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxuxbpnra.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gfiiwabgy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gkbytwfaf.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/guaioectc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gvkycmlmx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/guxgzkung.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gpgnlpgax.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gqoqnuceb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gxoueujze.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/golnodizn.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gpfzoomvi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gmhmdgrdh.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gcqvprygi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/grwoymouc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtmzssojv.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gbgbcwsrt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwcipwfqm.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gdfeshzmn.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gvqdvytxw.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gpjvszcua.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gixhamezv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/guhqkpttr.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/ghhfwjpdu.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gglxvgitt.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gyyhjfizo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gcgoxqenq.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gicsmcnzt.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/glecjfqbu.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/grggmgjow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/glmkkrcew.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gnzogopwj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gjrbippru.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gbfpupkbn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gsvbgkdqs.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gknmhbvpe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gsiydypfu.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gxkhvcfsp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/ghflmvrpx.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/goyfjvdku.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gtptdntkw.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gldoolghh.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gisqbxjdl.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/grwzwlrku.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/glvutsiyu.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/ghgfttwdd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/glykgovty.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gsbsizogt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gewbvdccf.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gglrqeyid.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gkawtuxnq.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/geawwggwv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gdxlgvnvz.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gnumqxwyl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ggkjtslmb.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gtcausqyd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqaantcim.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gjlqcicyf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gprvwcfhn.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gjdwudodx.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gkufjrewz.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gzxlxiwmg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gunbpapjb.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gllorfxix.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gelcotxli.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gqkqcoago.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/glomivkqj.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gpxdjqxiz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gqrbmyzfw.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gccjznxng.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gwtzpugwz.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gdduwatso.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gweacgzfn.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gatzkyuvg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gjfsbwjrf.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gotqbbwml.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gfnzuuzks.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gmwgxpsqq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gyytjzkgz.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gztkhnflr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gpgkobtat.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/glimhjfuj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gfqfjqaes.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/glejuxtec.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gfwpggqgd.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/giotosnsa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/glyisigcq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gsqlgumvr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gmccwihim.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gfwjltlnl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gwyxtiwly.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gissncpmk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gwbcyzocj.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gggythged.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gxewgdzom.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gytsocqch.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gpuodwemm.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gkmsjpgqn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/glzxlyttk.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gsdqcmmcs.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gvdjymuhf.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gecqpyajv.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gggjbwawi.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gjnhjiwtz.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gbreenhpf.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gpcqcngxz.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gdwlaqekk.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gbtizurpv.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gqqkunwce.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/guznarvpn.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gccdyjezr.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gerhflrge.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gzgersvne.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gvbhpxjty.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gxdebaotl.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gfwuhnxgj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gtxxfhqwx.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/guxnsnefy.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gaxgjxznr.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gjkgevlra.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gjcioujap.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gotjqsksh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gadcwsrzy.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gixooydbw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gnvtlihsy.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/ggapgucdl.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/guxgrqalk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gcwxhunzy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gdcckvvdc.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gasbksnlb.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gpknntipc.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gsgfmzuse.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/godrpypfl.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gaqubvgpw.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gmizotgpe.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gnmkdxjgi.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gxgkuubnv.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gpsbvcehn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gdlabkrxa.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gkijwrkhq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gmtmgiyen.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gqycyvtwq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gmxtzdbny.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/giwcbbhgi.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gtdbrryqq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gkqhkwlyg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gozggwutp.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gesbhwzyu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gsuxqzbkp.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gpotozbti.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gxbgfvcjl.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gwxmdcjze.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gjaiuxocf.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gpvdcciia.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gqlrmfprw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gyevtyity.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/glonvlqmn.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gmvngozsm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/glolcdona.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gmasvcrdo.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gqjlpnoey.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gzkursihz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gbaepivpf.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gcpasxsog.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gxaziwvjk.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/getunzrwi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gdovtuylg.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/geetahobo.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gmrjfqlav.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/ghlxhdtpo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gfxjiegas.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfdnbcdsu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/glvrfflhs.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gajeafnza.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/guqhnsvvd.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/ggchvkjwi.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gpfvmgxvu.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gwwtnbczy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gdbpaioed.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gdvsregkg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gqnqtnbvf.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gptjrgakz.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gfcjhyswd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvboxevut.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gwoxrjyah.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guzjovpmr.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdhefktti.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gzojukwac.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/ggyyrquai.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gdbjmzavc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gokwvjmzc.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gygvlheyx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/ghkhffvwg.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/ggouznjyr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gwowdyyji.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gbnrgpjtj.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gnagoiyzv.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gxybvuakh.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gumcgjdow.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/giptzrxpj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gmmdvemmo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gwmveedzi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gjqeeriyj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gftnrbcrr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/givwidwdk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gizlrkbwd.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gpadeqvit.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gknepkcvf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gfkcqdffr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gbskyqeyp.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gyloiixoc.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gjidqzukd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gficxafpm.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gbzvbengj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/ginzjzqwg.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gngjbeutf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gfezrwnte.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gxypzfsir.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gnokairxt.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gzrhgrnpx.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gtqqkizsk.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gjlccfodn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gkbdklvvx.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gilbncoju.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gdzvjykir.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gpsepeplc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gnmihcwsp.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/giskrjziy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/glilnqlou.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gpumgpneu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gkkanxovc.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gyuafdjvi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/ghefqjwoz.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gxxkpodjq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gqlhjietx.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gxlqdfstn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gvepqjlix.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gedxmmhco.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/garzwjwjy.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/getfvgoyo.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/guznbhqjl.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gaictfiyp.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gnveipuaq.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gyluufrfo.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gpgtrfflf.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/ghxmummqj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gbgjmjxsh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/goldnbfxz.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gsrnzxzvq.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/grsqqrjnb.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gnklteyth.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggmbyzdri.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/giqypyheb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/ghfehvsfm.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gewtzeltm.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/grxgrrmsn.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gejloqpcu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gdklmieyq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gsusncyef.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gsckhsnzc.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gbwhwqkin.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gttaxuckd.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/ghqcizthn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gdbusxzpu.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gtkkgnzpp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gljgqtegq.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gwdntklsp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gvnwdmszm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gclzofloo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gyqvtqits.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gpimzccxb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gvnulvero.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/ggfsvkzyr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gxlpjbcbk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/goxiymqjd.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gigohrycs.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gofvdqgjw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gdaaqmhab.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gmyxxhvlr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gwwioigcm.sHtML


<!-- 参考信息 -->