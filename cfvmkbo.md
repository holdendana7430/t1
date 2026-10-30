代发 wailian999

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gjqtwlxte.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gvioqwber.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymurdrmq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gheulgwos.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garmjkhcn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbrdsaex.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gipwzoyiy.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjgumwct.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqffeyumc.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gskkailgw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnuvdmif.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgvycmti.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gmcomjlws.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfiszoeib.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyswpccc.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/geartrwww.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gelucbikt.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gmhrifklz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/geadeectw.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcxtdtbjg.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlxuhqjb.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkgjajgg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gapkrfxhd.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsexzpmns.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guebkpvua.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gqvrwpdzg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/godvehhho.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxpnxaqt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gnddtngtw.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gezeyzjqy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/grzqrewyn.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemgubvmz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/guflezesy.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhteifja.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfvvxjewj.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/grufhpema.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gynksqnoz.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gyxwptuyf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewaqiqzj.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ggwjhgvyf.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyffmnngp.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpexcxcy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyaxaguz.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gsacabvfa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflizdzxl.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gueuzvvti.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhqkppyd.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gixnfqftq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvoipnvt.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdwtkglpv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/glgytbiqc.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjhhowtv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyypxaogm.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gbzqarwaa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvthuaoll.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gauagcfff.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoxkvphq.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gbpjuejmw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzoswgmgo.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjoqbvlv.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxspsrsj.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gqdzfyuou.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvqwiucu.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmkgpxhbm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbhjppdsv.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvtcgmek.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggygfqtwu.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvmcmmcd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gywfdjrvc.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkepftyie.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/glemmammo.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/grbleyncj.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goamkishs.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gctccrejz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/garlbslmk.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/grwozjbyn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbomkhiac.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaegsdvc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiycuqwc.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdowavkwe.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnyyvrigh.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gvummasbn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtumdbapa.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gflidfxwo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcvyoafd.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gtxvejndz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzbonmnm.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gtqlzgbgr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrwjtfsy.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrqywwmm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldigehvq.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvjmpgyka.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbggkehax.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gaaknihxv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsprdyka.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/grhciznxg.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqhuphwe.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gzghdzuel.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhqlfulz.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gespupsnp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gvpebohfn.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/grsrkvoss.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gldnxbjjo.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpeukhfqv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkijythg.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhakklnw.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geotmjeok.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gngmjkucc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gecshaslh.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gzspsospc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfucvthf.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmnpdech.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzmidfwo.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/glgjymkpv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gejlmkjhd.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrwhtjym.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/guswdhojo.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gisxrmkki.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjvmwdrb.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjgcfpaq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gfvsylgcq.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gypkpyrso.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmxhhhwk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbckqxwmf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/guhqqfvnw.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxpwzttv.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqiamzag.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqzdmcmu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gngimgdam.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigpwudlp.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvsxocpm.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gliftrnch.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxafonot.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gssjyimqy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwixrzxa.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gdaltxiew.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/grpbzxrvi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdnfaeon.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gicqtkaaw.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gfrhctehn.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gypmouezu.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjthgzzid.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeabqtjo.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gjhqalmei.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gbwomckug.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gftwddxds.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwyrvsiu.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaaybjfk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaprlcpwg.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/godoootzz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefpquvom.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnerrmdog.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/guqfzmxwe.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gymkzizjh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gegkkexce.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbiyterp.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/geyckpfnt.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gyjphlmgm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpqsukem.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gothmsckn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gjuhuvgzw.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gfjvzkbsg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnabcugoq.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvwlavdu.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnanfzpu.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gwcdvwyiz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxkwuzdve.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gubcvyopp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/glihrfnar.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guzltwdtq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ghkiikbhv.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxvhlavd.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjluawwdl.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxdeyfkx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glkpkbwzr.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/grjzusvkf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/guyegqwuf.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxijmsjj.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gytqipupp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grfyvctsb.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gtchiiniy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyyeknoo.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzxwhfyco.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwgnukrj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvphuytp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gksjzmzzi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/ggjclhmbh.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfwndymd.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gmdukjjab.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/ggyauuqqh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/goydgsktm.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxiiwubzb.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gndqndlyq.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gwptxjolg.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gccmftabo.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gzliqvhkw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbxetede.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gxtlccphm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpqrcidc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczqfybbc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwqwhaom.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gheicogsy.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gotbhzwsz.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdjoisle.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gyjlovxbj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gfysfruuz.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gbqocuhso.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyijobfg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/glppnbukl.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqephtsez.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvjmgyes.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmtcupwn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/germtfdsf.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkvrcssy.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gnodwcsgs.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwypojtgc.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gahlbhspp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gkqynytbh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gmpanoivo.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gceylyvzq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/guoifolzz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnjdukxyt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gqkjkotkp.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gmbcrxhux.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gtcmmgdaw.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gadqdsarw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/ggezwbmmh.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gajfuvcei.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gkmopgeim.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxgdlqxd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsegwiui.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gpounqwnn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxexxwcx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtbvsnvx.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxvcwdew.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcjbokgp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gcfgohrjs.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuwmbgwm.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/guqfqkkub.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkyvbgenr.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyrrmqjb.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmrgduqwe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gpjyzubrp.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmdemvdl.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gumsdoakv.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gslmtuzcz.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gxcsxvjfn.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gpkxprqhr.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gifmwxjjt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqakexpj.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnfquhvai.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfhkxtqi.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/genmdevvn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gbtnktmlh.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauoatbqr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcofhbfpx.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/glrtinwub.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulrrithz.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gcljmuync.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grubxohes.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhnnvndl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gctzrbpit.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtslghwp.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/goiqtoray.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfitunckr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzyppyve.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gepoissuc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grccyqner.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggpmvqxrq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwwopyto.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gibzkttoi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbqbynjb.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoxpxlyf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gmoludjrs.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gsysnaspk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gykddtevd.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gjipoxqpv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gsyqdtxps.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/grelyisjm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxraeegln.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gqafqtzjf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfxbnlcyo.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghepsyvfa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gdkxkssgp.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmjqjpohw.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glngrumfo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/guinqlfwh.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqcjzcsep.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gntyxxygq.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glgqssdxy.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoyqtrqz.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqlamtos.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdrutxfjm.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gbmbnckda.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskocgaiw.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gyxqkrhfe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccqdmdwx.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gkknyyebf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdituknub.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/ghjymkngf.sHtML


<!-- 参考信息 -->