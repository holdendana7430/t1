代发 wailian999

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gtorbpxwb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/grjmqnnsb.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gqdsutakr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gmyhmzrsi.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gzfcyhjpt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdenzchtc.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gnegzcwbt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvtybqlbu.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gltsxcqxv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjgvnzdwo.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gtlmeqjsb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsntwcyuq.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/giqfrdymn.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/ghejttavl.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gielbnykk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/guhhujoau.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/geyqnyybr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gvvcuioxb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/grwkfmcuc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gqzxjuhig.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gvxhdxjey.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gebnjbmhv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdahqxsft.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gjcfifojp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gjmbroxrr.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gtmrtngtf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gihowqrcd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxksfffxm.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/giyrhpszu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxtgyqfel.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gdqotutiw.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gxptpkefx.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gjmwkzjxb.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/goyucxjro.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/glywtizkr.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmbpoezyg.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gnqwjhvce.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gtdcaxlyh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/glnmhydac.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gfnqgjnfg.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/guopuvyjl.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gllyhggbx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gwoxsipca.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gcvopzydt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gsjtvknpy.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gewfpbfih.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/geeyrvvzj.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gallhkbph.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gmtwcrblf.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gkfsyoyyf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gzobdiypq.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gyrgfhxol.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gpfkmmery.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gndfxdbgk.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gegulseam.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghgobpyco.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gwtgcknvu.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gaixruccs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gomblgyca.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/glwmcvpja.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtcxnicjn.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gqjhqbnza.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gtmjdwthl.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gcrpebjtb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gxkduihpx.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gbondqxzn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gzlfzurpx.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gxakzteoy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gsmecgsdn.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gasfisgws.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/geonggsso.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gcdofymow.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gmhdcghdv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gfxeccmhr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gzqprjdtq.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/giyfcwcmb.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gjoikxpiy.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gtgqcfmve.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gmppgcims.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gozwqkira.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdcducukx.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gzzbpephr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gqintdsab.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gtpgsnwdq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gxgoyanmd.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gtyxebjjv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gelczadiv.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/givybabqw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/ggytsvodz.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/ghcrtdjxg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/ggkxmbvky.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gbbrrkjot.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gzgoecfoh.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gkyhobrpp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gdryepwoj.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gcitakagi.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/giluhkklp.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gusujchll.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gkcugkmud.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gvpxckjpe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gzojmwqyz.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gavevwhlh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gtzrynwed.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gdmqlqcar.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gqhbzrerq.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gxexapmhe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gpajsxavh.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gkwvcxndf.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gmsfqydhx.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gcygvhqcx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gqkzqvlft.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gwesbwjzq.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/ginruktem.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/ggmxajmzn.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gplohxnbv.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gxvoknyei.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/grzaayxld.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gisbjibza.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gyjgymtjv.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gtdwhepzu.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gwnnxmhyg.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gqjorbpyp.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/ghvcyhcwe.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gndupoigc.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gzpsoyxmq.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gpmgqvlyl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gdkhqvlmg.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gfhjyxsjm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gpapaajuy.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gjpjgnfqx.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/glaoesujh.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/guirgrllj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/goiukiwec.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/geuuwqdqd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gcslarkyg.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gaxpzgpmp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gbqydsfmv.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gdpvqinix.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gwlalaykv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/grzfdativ.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gtbhftcbt.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/glkbjvwkg.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gtrjmnzob.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gkurulmhx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/ghsgudgxp.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gublbfebn.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gisrnjfzy.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/giebmniwb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gifhqkmmn.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcyvpoilc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gjsolaluh.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gudcdswjk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/geqcsyynx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gjquioblq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gdftictbc.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gqyrsqvyr.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gcoaankjx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/ggbtydyie.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gvlohzzfc.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gpmhclzzx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gnoptfwmb.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/goptyytah.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gqhyimlbk.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gsynvzfss.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gdfaxyaia.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/ghtwjjmbp.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gbmcjlmhl.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/ghhoxxcud.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gqfiqtuwc.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gsvyehnin.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gdvogpmdi.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/ghefiehry.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gfzqvbyif.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gudweughz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gjqngeaqz.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gqrlinkeg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/grscfvefc.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gkzgvxion.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gklxhygar.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gneemqxce.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/grwtsmvdi.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/ghiqrbbat.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gppilajsg.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gafxuvnvm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gxqieeuyo.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/grsbccpgg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gfjsskmsp.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gqpdbiiik.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gasyfzqkv.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gerjyxmxd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gzyhlnick.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gfpcmnjob.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqjsxnlwf.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gbwodtomt.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/glvvwzlxh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwzbigvyq.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gmbhocclp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giqdthyim.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gydbtdiyw.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gzybyzinn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gpcqtzblv.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gdfmarldd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gjgwavlth.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/glodylbbj.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gvxmwyvlz.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gxlaegcqd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gdljrljrn.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gmdxohxkc.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/goqnlghdr.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gguxilhvz.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gnyjlvwyf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gugjihrso.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gvfntcono.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gnoflcqfb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/grxmtzufy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gtklxmmdq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gcomxydrc.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/ghxtetffd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/glvdziruq.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gfwvhuwiv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/ggunlbczi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gcbrunhfu.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gbawweejl.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gkzqrlqyq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gmqkpfyxb.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/geqjvxdkb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gyxwitnex.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/ghuwweiwt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gcwdbigho.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/grlrwvzld.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gpmjnbnsh.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/grzjruwcu.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/ggirtslai.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/geolsjjum.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/glyqlaxvn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gsstktvwc.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gepqvdbuo.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/ghtaztghr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gjvytqznz.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gvmptcuoc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gjsnjqgvk.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gjceqmzej.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gdvzydaia.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/ggvisxvry.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gpoxwwzsq.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/ggtgfnvsh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gqsjbvykb.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gmvzkjmff.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gmwabemjp.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gcdqhzfog.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/ggfakoocg.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gatsatbem.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gexzipibo.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gnmrfcydt.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gontlawox.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gszdyqcxa.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gefeswlsa.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdepyrvpc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gjmoynoct.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gqaqrwyvf.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gvqtsbwdm.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gbnwlghfp.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/goftnazfr.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gdertxmud.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gmirdetoi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gudcxqfzc.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtcxfltfv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/guoxzxpwq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gnubcejso.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gycnfuasa.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/ghghsvrnx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gkiejjpzd.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gbknbwrlu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/grtypirsu.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gprgliixq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gwtbdueyg.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/ghkkodzhz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gjpfsyzse.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gjzsmzsvu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gqnsaoxfs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/geuafyvpn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gxbgntarw.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gebdoqczy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gtvprklth.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gzxutjlau.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gmjrzujjd.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gfuzaorhq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gictrytto.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gedfrqwhn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gwldbdpqz.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gnhrxylnr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/glkqjqqwm.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gdvxsqfbv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gnohikqqu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/ghednyniu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gdnmlxejv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gmizuiuwk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gpbuktodx.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gasevctxw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/ggbjhhjxf.sHtML


<!-- 参考信息 -->