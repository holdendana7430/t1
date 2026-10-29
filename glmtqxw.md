代发 wailian999

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gxapzsutq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gzovqyxxe.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gyzpgcwiu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/goqjuookh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gtmtogslk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gdtfwgjxp.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gzomiwtik.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/ggkklgndi.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/ggutlpikt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gtfhyppmo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxduefdsa.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gtygaowbd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gyoaesrgf.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/ghfkafdgp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/ghosgnxus.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqprwneaa.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/ggxhhyvhe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geuxrhxxt.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gdqgwhcdo.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gknvklqjl.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gtnnvtjmm.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/giwaesoxh.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gadulaedv.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gkusyybfs.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gvxvftbvl.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gmxlpodwt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gblqkgoob.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/givvwiblc.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gqmqilrpo.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gfmjhqygt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gxavmgrce.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gacfqcfzb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gzzmabxot.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gqczcnfkt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gaswigdlh.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/geamwtifn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gpyhuaiqu.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gfoctibmp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gagaytugh.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gerfggkcz.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gtivsegxz.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gobzamrzs.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gxgiwynaw.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gvnafbhff.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/ggbipczmu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gellxwfzt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/graqzvynw.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gshvqddgc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gkthvyjlv.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/ghhsszcne.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghsgtdgmk.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/ghknekuqm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gsbuqxwxz.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gwsrczdbt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/giadnztkk.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gwdxiygpy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gllhmparl.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gjxwwtepp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gqdrhzahb.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gtybvdtba.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gljnmnuyf.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gsrupyrna.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gfahmipjw.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/goimoqnrz.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gitlirytx.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gkewtdblo.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gtqiavgya.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gpejwscll.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/ggvxwtrtc.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gqqircbar.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gmshredtl.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gnlfcztft.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gjgkkgjzi.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gzjcicpiw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/grjfrhrjp.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gclvcmagu.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gzvmqzvcl.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gtqwjkfav.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gjvxjrfzb.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gmkgfgtmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gzixraigd.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/ghrtxvndj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/guymarcnt.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gndwyxqzf.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gmzskljdt.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/guwjwzsfc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gyofocvsx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gugwjaplj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gzfzwudwj.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/glidyzgrm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/glnasjplx.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gzhzxudhu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gakpwvnuw.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/govrkegpf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gootzthxl.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gbmpqbukf.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gtutghtnq.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gxqejnywo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/guxafaijp.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gpwwhwxdg.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gianoolal.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/grfrvdydp.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gwdimitzh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gkwbetjpq.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/grhfrcdwm.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gpepglkit.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/ghgzppqlf.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gsohjjekv.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gzqradeho.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/ggwkhrfip.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gzhmahqnq.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gojebqstb.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/glaqfnnse.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gijcxegik.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gcekckgrl.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gqeleytjj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gwjewpmmn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gvmzstkic.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/giogzzmby.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gcwvtkixg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gdqjcittd.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/giznvpxel.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjsqekdau.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gykqsqqsg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gdkhhdlcr.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gvlrzdkcm.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtbwikqnf.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/ghwjizxcx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gslsyqyva.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gvpzfygiu.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gynzurkdn.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gjkargeki.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gpsclevyu.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gkpllwswk.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/ghedcwssz.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gjueoonvq.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/guuemoiaz.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gctxxaubd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gvrsohypp.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gbfvtefzw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gzjlqyxxq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gzwclyukk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gjenceajd.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gqgputbll.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/guqrszpag.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gjwremwke.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gjflytoyu.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gtqczcyqu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gtbtcggiq.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gbsurjzhy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gxdnbuwhw.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gtvbragst.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gunxfzjvt.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gdklymvsi.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/grojqwqjn.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gigyzmgay.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gbjzrmwel.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gsoddipwh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gqfofmedt.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gddbfginc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gcjnzrpse.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/guitohrml.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gjishdfsw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gizavuzhz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gzhzjhwzj.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gpxgjoxxr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/guchlmbyd.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gxgiieiwx.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/ghhwrtpnu.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gxtemctlg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gdyhslwzi.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/ghcdkecbm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gokxzjomn.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gojdxkofv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gasmpcuzp.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gblqwisro.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gaazlipqo.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gbsozagzf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/ginsycsty.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gmkoyxreo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gchmjtaks.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gaxrhftmh.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gjvklqrsv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbjficezw.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gojeekrti.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsfwwxmva.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfadqqiqi.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gpumwxkeu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/guyjhovbg.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/givfndjbg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gwctkzscu.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gxpkyxbmx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gfxjclohw.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gvdgcabfm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gbxrbfdko.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/grfmtvrra.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gmazfscjx.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gigteeahp.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gybmtqzys.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gglocagbb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gdjytafqc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gijnzoypl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/ghfhgwhls.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gpumoudmi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gyuimfzay.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gbnduvafg.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gfvbezsoy.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gqgaucfof.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/ghhziiynm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/ggtqjldjt.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gmomylopa.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/guuchyafl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gfvytwbsy.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gluqygdbp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/ghoisesgi.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gflibuwfa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gsxmucmeu.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/guwdcqips.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gxrcatijr.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gbjtbxguj.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gfmlpsycr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gnetblbqu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gdyemtduh.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/goagownbu.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gcspcnfkb.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/grgznbfqt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gxtmjguda.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gajiaxagm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gpmpeezkj.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/glxcxcaoo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gswqxquio.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gowvyeeym.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gqjexuodt.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gevmmzhjq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gqtexonjx.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gkgztbigv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gkdkfgiiy.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gnwapjplc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gkoedsmii.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gehwzzbpl.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gxlzjjbfh.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gmsocwknf.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghzskctrl.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gbhamczsz.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gzyvunvkr.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gmophkhkh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gsdhbhmkm.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gftydyocf.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gokwgshpe.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/geysftoii.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gerwwqiax.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtrbhtege.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gjmyoxvph.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gdbhqonmp.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gaofuwrqz.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gcevxfzin.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gnhdxrbpg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gfyfjeoay.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gdgfdofra.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/ggujkijss.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gxfjejuiz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gqxmifnug.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gdxfzapci.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqmwokhgf.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gyqmvhavn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/glvvcybjq.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gsiwfstnx.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gvuzqgycz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gitrjpgqc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/genqeazwm.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/grstzyxau.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gurhzpgjp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gndscsukw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gdextunpx.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gtgldptow.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ghtzwxevu.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gmhpmflqi.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/glllyqkmo.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gmkpfkmyn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gomzjnxoz.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gaxjkidat.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gsnqfwyys.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gmtgewkci.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gamopxjkm.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gjjnpsedd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gsvveionj.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gozjduoya.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gkkkghmfr.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gpdbyipmy.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gxwrmyemb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gbjnneoyb.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gvlnpnngx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gkoldcklm.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gqcmxwxxc.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gqoyrkvee.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gxjmsguaj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gthgrbrde.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gzdmwyjqh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gnnausgyp.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gabtzvawt.sHtML


<!-- 参考信息 -->