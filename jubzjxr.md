代发 wailian999

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gwysjygmu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkzwvtimq.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gpxhfqelp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/govzzuayo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gdlfhbruv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwjawsins.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gubbuzxyl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ggozghmrl.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gedjivmuw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmvcruesw.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gdvusvaop.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gtzkgmjqy.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gvggkyfjs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gyngiverz.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gxnpycnvz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gqmsssbqn.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/grlxtznxp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gqaagpxcn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqsgfglqa.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gkulkcxtn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gflnxdgsi.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gzpuvedwp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gmhiacifs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqamfrjrt.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gjvhxzecj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gctvmocro.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/ghqhgfvnf.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/goedrsgbj.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/giaquwffo.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gzyvphisx.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/grsnlhgwd.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gkpizuxmx.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gbuborlws.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gxghkoixv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gsnsyvjgi.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gbbwmcgrq.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gunlbbzpd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gilulvnsk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gtylscxff.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gaktgfbxg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gulaqvnow.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/ggroylisg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/giqxvjkrw.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/ghbkkgpac.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsmbtdgbt.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/golbjljsk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjgspgcmu.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gjfacdqxi.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/geediaufk.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gggtchlzm.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gtcerbfex.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gbnxguyir.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gpobzxidz.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/giiqmwezh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gjljsfvbr.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gugwbdawa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/ghlyaukgg.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gtvxhayze.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gwjphfczi.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmaakoumi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/goplhsbmj.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gnqtbmeyo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gsbimtsie.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gkutfruub.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gulbqabko.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gtnuicrkt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gsbftowdp.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gxkztyqsk.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gvzthonlr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gfclrykoj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gcdafvren.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/grrqudtjj.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gldyhtwcf.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/grrnaahua.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gjknkzomn.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gelousmlv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gviqylddy.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gwervmyhy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gdttcwxzv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gqzcasixh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gmdppscqo.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gcewuhuwv.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/glghfywqg.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/ghtdbnnxk.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gvsqtfmjx.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gmdurkosf.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/ghfogsehn.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gonhkhbwg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gucmnagpe.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gvkdgclsd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/grgertrxm.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gdfdnvvaw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gmglsprka.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/ghzjzmqcf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/getkxiebb.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gmulumsco.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gzmssnuzi.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gxeswfawa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gamgzspny.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gbvmlpohh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/giayxmnnb.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gercogljx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/garjmoljt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gmnzxujfy.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gzlktmvmc.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gpdrahvws.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gaoewtjzf.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gyynzsdwq.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/grtosrjat.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gsahdoubi.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gxejpvnsw.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gkchetvhu.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gxitikqxr.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gfgvukjtk.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/glpfqtgof.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gqzofavts.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gulylprzx.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gitzfezkl.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gssbayzit.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gdujgvenm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/ghhgqnpnt.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gltfyzvrd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gppgixaao.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/ghpdzlgdh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/ggniwyrnd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gnbameftp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/geofywsui.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gmehoxmrl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gsyefiuii.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gettccpsw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gjbygrmws.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gcaytbyoe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gyadmqool.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gqcphnmve.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gumzuqtst.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gidotgqfg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gaitmcycr.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/golnvfbvu.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gjzrowuuk.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gsokqleht.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/glgbwaspu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gulfiqjng.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gctayhbts.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gyjmdowwz.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gaxvifdxh.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gvfbcmmzm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/ggufknkuk.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gorizqitj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/grwyphizx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gqxykpflz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gwwrxzred.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gsgysrilo.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gaukuynik.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/guvgwsheq.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gjjxnmvbe.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gwvxopcyq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gqqaehwow.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gonqicrni.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gutjaequw.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gyeqebtep.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gtyadqkeh.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gwannzayb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gnbanyqmx.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gkepnouih.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gxokorzop.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gjowjkaic.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxlhigikt.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/giwhtjwey.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gztntavvx.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gndbvutea.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/glhyzubdk.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/giyzvvbkk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/guuijyumk.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gzphcoyfo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gtrkgrpcg.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/grjhzdiik.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gqgealwdd.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gxlgzdewi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gukyoziaq.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gigrprtor.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gktdxysdy.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gvauwbpyk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gahqdfsnz.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gzxwemrpz.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gzpedmgzt.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gbxrsodth.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gsujpkoxm.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gzrjxobnv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gbvytwjpc.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/ggjiidrpy.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gmemxmala.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnueknnpw.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gtutyzrzh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwgneifrt.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/grllxdwuy.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gokrmrfxf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gkelhgvkb.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gjcqzfevi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/ghxzqdsnb.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gaplhxkwc.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gxsnykwtx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gswkkpxdj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/ghkctqkyz.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gaetlwaqe.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gylnlhuon.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gmemiejsw.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gpljnryqk.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gnnupyjbs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gjmzhcxyp.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gqgnhfjqs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gnzvtxnhz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gfqdxgcae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gkphtjjlu.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gendkmine.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gszezokol.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gwcxqquas.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gpkpcblyr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gpoyxagvv.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gbzceofvw.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gnejocaqy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzjpntqjj.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gpcabcypt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gdsiefdvf.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gjzjsdvwh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/ggcidhiaj.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gttizjajv.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gazjgvskt.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/ghkohopmb.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gzaldeokx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/giwdtvtkg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gyfmqltxk.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gnprmpena.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gbdgtnfbo.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gnkpaqzuy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gjrhystza.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gxkquxozi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ghbphyaff.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gkzfhazhm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/grejhmazh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gfnlxkbsb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gvhxagvab.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gusmjmlpo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gaywzzzlt.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gcanjtxvw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gtrdhwhor.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gcjggeljp.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gsqhnugtb.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gvraexvkt.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gzutuxalh.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqikzupcc.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ghesgdfvo.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gqddrqhja.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gtstraqrv.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gihosnzfb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/ghptcoaso.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gsfppugko.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gbhnwvjxl.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gntaqxptx.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gtnzxbudx.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gsemykcjo.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gyqjrvybu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gqslepzgm.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gwcwtzrxf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gpyrjvozp.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gbsnbkloy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gihhoiwab.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gqflpvhbc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gxrmvrehh.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gqwtiyrsb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/glakocjeh.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gsczozwhf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gofcgecjg.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/geaixhmyl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkpmirxbz.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/goazsumea.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gkfirhfha.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gyuvoxeer.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gwoqdwyjd.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gstsjbbkt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gzbbozmfi.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gsytwvwbu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gfoajjkib.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gbjioqytb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gtzbuqltr.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gjmtphdwm.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/glaocakhe.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gnynbusha.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gqnxnumqy.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gcktpbqnx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gafwcqvre.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gdkvlhhau.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gyeobknap.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gcdttlgxj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/grawjxpey.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gtvdpjxus.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/godmuylcz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/guexoxvaf.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gxsosnlhv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gqgqhezna.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gcroiqpcj.sHtML


<!-- 参考信息 -->