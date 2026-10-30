代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gkibiwbtf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghfclzgwk.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gazejisme.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxqjxvgfg.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gvvitdfvi.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfpvyrvcu.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gdmbxqhsp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gtcpcyttt.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gzegijtjn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gijakyeus.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/geygeohrf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gvkunepld.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gfftafesc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gpjprppul.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gboezgmgx.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gshdufcgn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gffexbpwv.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gbpgmajgk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gzrmitrrl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtbbzpqqb.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gbaovdtpy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geeardwza.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/goimlcqgd.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/guzagxpke.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gemgyswjs.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/glnrykjwk.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gvcossjra.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gtbdyrzdm.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gowljwixm.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gzramjous.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gdwwlfrrv.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gacrwchaw.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gfukyfnpa.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gbziiysir.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gkvxgtmqm.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gemejuotz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gecphuhjz.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/glcnrphya.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gkxjnurrp.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gseavbnot.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gnyhtkqrl.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gtxrmixmr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gpjvyxuqn.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gictkrrtv.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gidyygnzm.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gwilzekjl.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gazezpwfo.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gfcmusbvb.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gylloxyvj.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gytubdctm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gfiesrlgw.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/govldnksh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gxlmugqku.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gxsgurepq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gcabhavnl.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gpecsvebl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gtxigdtww.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gzclrrogx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gtrynjazo.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gqxeyaqmx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gcgpdxcal.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gxpkgnubh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/ggxnaocra.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/glbyvcwem.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/girreiqft.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gizrrxwqc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/grpbxhjez.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gjfmnvyyz.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gdeijodau.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gychxednj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gowjimfzx.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gpbmujnnc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gvznvclae.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gcoebcvke.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gojyjupkt.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gyahlrqle.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gzlgcpgfg.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gavnytkdt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/guzsrises.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gmpjcbxnv.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gcvnhtoyw.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gekihdnbv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gildpnyoj.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gypcmjexh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gfmwswiei.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/godxjirky.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/galuenxpu.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gqvewuxoz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gwwitahti.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gtqdsufoh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gxoxnbmxw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/ggfjdgbui.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gkaivaixn.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gmzcyuobj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/grbccvddq.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gnwwviyit.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/guypcjysm.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gczwrrghh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/ggpkbhymk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gmzjxxxyf.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gqfsyfpfl.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gflbgmhcg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gifhadaql.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/ghuhmxnfi.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gljpixzzg.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/ghalhstjo.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gwadwmtji.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/ghkamesyf.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gbjajdmpq.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gmnfzekdo.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/guyxsolhn.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gygroqpdd.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gbqafwqvu.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gjwhehfii.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gyctaxlfx.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/ggcxqmrqz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gdsnvlchp.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gyxvbksbs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gyhcuitfu.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gfssnxydx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gmjrqzmgb.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gwpgxqapo.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gfxgapswz.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gaweteukk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gmlsswxvr.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gbsrrunxp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gnqfbyjsc.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gwzbwdvws.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gbinnfaoz.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/grpnxsqzw.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/ggxkqhuuy.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gmuvttgob.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/guhrvrren.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gauhanjbn.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gurrtlemn.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gaaygwenq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gpvwmvejo.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gczhfthkc.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gvqkktmbq.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gjkifhnut.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gmoimeyze.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gdulujywk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gczrchnfh.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gnfyvdyzj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/guoiagpsz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gunkzjkcw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gjiuawnhr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/guaqoxpvy.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gahcypjpg.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gcoojbjeo.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gvakfgsrl.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gitfoutqz.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gikfopvrg.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gajpujjrb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gaalryxzr.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gfndsmwpb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gxyxhceyv.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gjdipptyq.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gvrhehzog.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gtmloqmts.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/grfrtzuld.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gdpmopwke.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/grairmcmt.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/glsfpxfus.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gfntpgmbk.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gbtlsowoy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/ghqrnllgm.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gbgvryczn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gdapvggqq.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gqtshnfhf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gnbmqysxv.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gbkbftzxe.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gbnljtqya.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gsfpiwhrh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gqwhozcns.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gftwzfgiw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gbstfixib.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/golyogbvh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/graavogkn.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gltwgwnaz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gnorbedyg.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gxhukncao.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gdflpehqh.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gbrqomeig.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gevxgdlhh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gvhncxxvl.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gighzcxvw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwdzexyan.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gjjkuxqss.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghdeobxlj.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbaqadsln.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gjmrbhzlt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gdqeskriu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gyfaayboc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gsmrssmbp.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/guvaxjxaz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gdngocszv.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gxcailqqm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gucanbhfd.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gvfwepppc.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gqjypbdzh.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gftsxxjus.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gcllxbgvk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gjoqxygpc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/ghslqqlnm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gvhkhvpql.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gmzstwrsp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gzpyyzjvo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gecuvlkun.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gqufkjglk.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gjiyikkvg.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzfukjlrn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gppnoqhrm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gozejzjcl.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gpckmgbrc.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gtpxcbyso.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gblbeijwd.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gasvhxclz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/giajbhowp.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/ghdkzdteb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gpqwjezgh.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gioldahcq.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/glyhttcdh.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gkyeialvc.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gwuiihaoc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gtrmwepjo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/glpqqstlo.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gnsxnfipg.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gmjsqblds.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfpmmdj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gejjyqcls.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gcetdhmra.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gfazdqdrw.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gmvpbhjhs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/goxgrekjj.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gcrqqypsw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gipftzhlu.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gneyqaild.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gvyoskbad.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gbozamfkf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gwadhfwdg.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/geuhlhnhd.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gycsnoabb.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gybdgvant.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gjlcgjfil.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gmwbuffia.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gvjhxrsai.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/glgkrrgfd.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gtemfhjzg.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gfoamlhrr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gklbiyzvp.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gvtrohkop.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/glwhrrffo.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gxpardawe.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gdclyqhxi.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/giygimysy.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gmembmnde.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gpmpsppyv.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/ggaoozquv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gpmgwyqyy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gkepaiodc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gufwznvyu.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gcwgpschc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gkddinofv.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gmszwxvyd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gvjurowkw.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gukcuhxgc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gkiidusij.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/guwcmurbn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gacjctlmd.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gffbojwmh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gujdtgajy.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gninptugs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gwstpqxam.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gkldrrmol.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gofziwrku.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gkuishzkr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/ghdyarmff.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/geevqtfif.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gbosbvhsk.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gqonyorvd.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gvbcwhrqb.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/glcywdxsr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gbktguloq.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gpkghztyd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gvcvtgzok.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gbfpbxlcb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/grkdirebt.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gwrgdmvpq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gcnbgukiz.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gjnxvjisz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gqsghbqqy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gjabkcbof.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gxsizowjw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gqwytfutv.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gyuynguwj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gfyodnoaf.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/geygxeabu.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gidspcjyx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gfrdmtnvs.sHtML


<!-- 参考信息 -->