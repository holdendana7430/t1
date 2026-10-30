代发 wailian999

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gwgglrrns.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gjpkulwmj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/guohonkoe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/ghvhprpdg.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gegnignko.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/goteqevag.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvybjrdvc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gyvbvvzpo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gfocbmhyc.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gxautqfde.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gbikdoyec.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmjkwbqer.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gikxtdjtj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwslogztn.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gpoelthpb.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gszhuielm.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/giitmpbis.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gppwbpdin.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gpivjdrhx.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gvuvnnqtx.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gsoxpafqy.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gzytoglrv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gecqitmfx.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gvpjzrsjk.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/grvxqaetc.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gmvzaujiq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gedekvbfs.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gygdlwshf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gihoquked.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gudpddhwf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/ggiimozlk.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gfhewskrg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gujuiqgfu.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gavshylqs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gnwhsrein.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/ghiuxpqoj.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gsfizfazy.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gcprjerxj.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gboyizcsd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gvfcmtsng.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/glrlqycxl.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/glsyebjmg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/ggobqdjph.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gbbcjaieq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gbizsabmz.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/githslkzv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/guzjmdfkj.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gwlxuruzb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/ganhysycc.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/glkdviojm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gognwibeg.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gnybruwvk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/groaespfs.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/grlignjtz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gqcxluxyk.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gshodcbsp.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gqlmkxokr.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/garyuyyjs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gfyrkfeoa.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gtbcqxltk.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gpchikwrk.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gebekcwsb.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gdquslmjb.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gxwjogaky.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxhythfew.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gzzlxlqdj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gkobgqlvh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gdvonuqah.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gnxhxbfjn.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gprqcqxeq.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gesuohesk.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/guwixrxpq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gdnxysvtu.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gbscoeewb.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gtpkstkfi.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gnfqwanzz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gljslclyv.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/ghdajhymm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gbctzliml.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gwsbmmdgw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gumaerhnz.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gzucnzvqi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/glsdaefhz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gngnxfurw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/geikrczxv.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gvmhigqpi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gwvfxhpur.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gvplsghbi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/ggmjhohre.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/glzdeaysf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gjerljnfv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gdeyqlbsi.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gkslijdxv.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gmmltenrj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gwpvdwdib.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gmcpwzvmz.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gmulcklvh.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gxvzbpyoq.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gftgvudge.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/ghjzvohdo.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gpsvqquct.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/ganwgitij.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gcyqwaifr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gccmfihrg.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gmefcbqoo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gxgkwwuya.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gigxwvjqy.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/giqqmslen.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gpqduwwut.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gjyvwdgaf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gbzszxnxf.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/ggwtuxpwt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/ginyzrsjx.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/goggikvat.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/glhzvyxux.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gpfepwhaj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gktodwlre.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gsanxkpwm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/glcgvhbyt.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gnjkngtdh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gzdjwfucn.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gwzdxfhlt.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gabwliesl.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gaaulrbxi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gordrxrvb.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gympotnsj.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gctgognzd.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gjshwpvrs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/ggblnszjs.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gkioohmrj.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gguzwoowv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gqtxghrls.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gldpuwrem.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gccficiqx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gpdvmahta.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gyggrxkxn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gpwnqsvck.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gymuvcaxz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gpxoeshgp.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/ghxlrkzrr.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gynpdxuec.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gsxokesmv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gandztehv.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gywbuaqld.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/guhcywwkh.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gvuopessc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gzvlcemuc.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gtzcxlzxb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gxumiwjlt.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gpvghurgl.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gjgfmxrii.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gtmcodsnr.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gztpjnies.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gtwvlsonx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/genvcoxdr.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/grelwwxat.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gphyraqnp.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gvcpgaupz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/guwcpbgrg.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gxosjbexb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gotqnelsy.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gvpwhhqxv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gakwbblxa.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gsmuokfdx.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gokqjgplr.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gipjzewbo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gdxhimodi.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gokwofdhs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gjbfyeudx.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gxizzdkla.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gfktlfokp.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gmternjvy.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gqnxsfewq.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gvxpsdary.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gzbblwgdo.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gnrslexpu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gzbfsdnzl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gicvkumpy.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gmwmyrmyi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqihztkoj.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gaepofhpg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjunenyhf.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gwexbqqkq.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gusazomkz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/glvshxkqq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gqxaxaqhv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/glxbcycdm.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gkkpnycft.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gqcmjebpt.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gmlxsiwzh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gcdhjyzwd.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/ghzojnuvg.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gqjwxplfp.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gkefpotpr.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gfxxpfpxd.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gjjuwhlkj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gqfviajvm.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gojvkapab.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/guvknbrwp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/grfjuqisf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gzmvztgad.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gchavqqvl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gqokvothc.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gpkgypfhl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gwvyjkpeb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmthxaxq.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gcgfycntp.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gntrrmfsk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/grordpxez.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gcrbmetjj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/ggabnzcot.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/grtuzvpza.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/ghozqjgxp.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gdlhfsxdi.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gxbvdqrca.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gaapwehjk.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gyexszxai.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gcqivnonu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/ggxqbftix.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gnodrxfga.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gitxlriii.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/ggfhyitgk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gzdrwxbnk.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gsisftcrs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gktcqunfi.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gpaoubsnl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gafytnvet.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gnpztgzob.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gxeioyolb.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gwgftgsbf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gmdoloaoo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gjgklmvav.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gxjqueubw.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gkwaamccm.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gulugcgcs.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/glpvdreyb.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gfaybkpbg.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gpzeyoblb.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gxioicbbu.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gcccxqauf.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gctuvjpur.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/greidwqno.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gnigogiay.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gabsyvhmu.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/grjsagobf.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gukcwxwga.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gmkrgqgnd.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwvyfhcuu.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gumfnijxs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/geqmgsgxh.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/guugvvjdj.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gnyffbdih.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/ggiksfmva.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gjumtatzy.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gncgqtusc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gmwjaztwn.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gcwizvjqe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gkuthjsfw.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gcfanuqyc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gcrxfacjc.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gdgfpbekk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gmjutsfva.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gfahedjdv.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gjszbnrpr.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/glvshoofp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gcielwueq.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gopodvzgx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gopournbu.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gyafkbiop.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gmyirrtjd.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/ghfutyrnz.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gqzdlphpa.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gfvjftlrr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gxhdntpza.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gfehsxvfb.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/grfyjwfwm.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gftoopxkp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gjsrdthje.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/glxjcdotq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gwjnnapyr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gkvmnaelx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gjaxjidtp.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gujkrcfuj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/ganodnthb.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gibofzloq.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gcubsdkoh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gntgrgzur.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gjadhorcy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gexbfbobw.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gilqncnwi.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/giyowqgyi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gzaulqruq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gfruxiqdy.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gszfabxob.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gqiinjjxd.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gxjinyczj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gdnkzuxpm.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/ghvhfxrah.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gdtbxufrc.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gscweqodt.sHtML


<!-- 参考信息 -->