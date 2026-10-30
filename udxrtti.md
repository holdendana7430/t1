代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gfshvfxyi.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/ggxqxfbfu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gqhispvxc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdeuwgfpn.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gmolyftck.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcrdostsj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/ggyquunhq.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/ggubiwthb.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gazntphit.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/ggnowagff.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gnzactdzs.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gvujxrowg.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gamxornph.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gapcdoylo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gymyihacl.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gjzeuxrqn.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gemiylqkm.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gryhfybgs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gbkmjzsxr.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gcnwlifad.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/glzjucaob.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/grqqjgfwi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gbsnluvfd.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gttzhlmdv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/ggjnyzmey.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gbmoxynhu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gwbrqrvaf.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/goliplhog.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gbkkgynqj.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gzlvuolnh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gisnkbrjb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gmumahved.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gowurrifo.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/grlyucuya.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/ggzloiqht.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gvlbyvzfi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gweqmxxym.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/ggldaonfl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gsdyvbuvs.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxjbwlkyb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gscinrtjr.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gzjaltfgu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gmjedknsq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gafpivavs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gmztydtxs.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gnrbdqyav.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gldrnvfec.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gmrpzkkrw.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/ghrmdlzuk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/geewlkvwu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gbhykvsev.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/ggbbqlnnc.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/giodpodfi.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gfazxjxhy.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gkdbgmoqn.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/guydeiryg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gqcvhgobi.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gacdvdnvn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gvipikdik.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gzrfhmuuy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/glxrahdyv.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gffcxkiqz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gvdzjzutf.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gxftwwthb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gyrhbvrpa.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gxglxuvwn.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gfgyqhdiy.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gkyrlxiif.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gpkauwbib.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gdgtlblac.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gamfkyyxg.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gzppqttue.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gltepfyzp.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gdwuuyhvo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gyzwcxtxl.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gkxqisuen.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gfwacuvbx.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/grxesyqzo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gnebtvnuf.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gnfcrlncf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gcrtuxktv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gffhkfocg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gqsidnjit.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gfqdgkrvp.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gtqcpunzw.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/glghvdnom.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gkokstxae.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gzpbwtvlw.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gjavpfafz.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gplugpubm.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gqknmmixg.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/glmdpxrjf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gdvnokheq.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gewlnompy.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gmknstuuu.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gapprnuzy.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gcwsduygy.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gbelfxres.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gelkmiwug.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gdolsnswq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gqmuinvqz.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/guuscnhag.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gvwbhfrtz.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gidrkpije.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gpeyblhvr.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gooohrhsp.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gjkizfggu.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gnwvocheu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gcyoupcun.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gawresytw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gsjmuavmm.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gwbqazwkr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gkrggwmtm.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gjpckdsdl.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gktchnxxc.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/ghmhwuucs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gdbahcvkb.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/grsxzfwla.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gbatsgejm.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gyeyajcdk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gdichidht.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/goujwmlek.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gjtwfbhzw.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gdvdslgnm.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gcxuvgefj.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gtnazeyxp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gwullxjlm.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/grevrnczv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gityklmib.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gcgtzrraw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/glqcgxgos.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gvmuoxeaa.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/glhcyjwig.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gxcuceeud.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gauysnwaz.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gmawbfboy.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gbgbwssfv.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gajuikodn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gfpabohtr.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gntzbusov.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gyighsztp.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gbuwmajtu.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/guvzrncmi.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gspdqdpqw.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gzqarnalm.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gzhjrbejp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gvlvxyday.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gzxbwyxdz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gmaakoyqc.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gddsikmgr.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gdilplgqr.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gqdpkgnaw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gofdhland.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gbwgvhhnf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gfblthjkb.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gvqhxflvw.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/geasiykzy.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gbbfqdrlp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gtmshofbi.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/ggqlyjtqd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gwkxmjzrf.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gwrixkzwg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gqjqhtzml.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/grjpnivqb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gailyseoy.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gbmpnhljj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnfbzbymk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gccatqohi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gjjeixzff.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/giapwlljr.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gbhtktwzd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpqrprzal.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gdhtacepo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnaglxryn.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gpirdrxvr.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gskflihfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/ghtsxwlls.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gsptrticb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gajessodi.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gcewopjcp.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/ghkxvmqem.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gnvwkpanv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/glmcgdcyf.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/ghvfjixls.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gqlyqwqxj.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gajkbmpko.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gywezzlry.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gksphtkpr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gtrodvtuw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gluwehsiu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gnumtlwpo.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gepiyolrh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gjgcypgad.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gxqfqcyqa.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gflexfxqx.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gvxbtkklq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gudkjagok.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gomdlizjo.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gsvdbyuap.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gywxxvzfq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/glqxgbewr.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/goefjuoyp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/glbkfdlai.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gdquqosun.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gbqjkoxpq.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gzoxjafhw.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gmpkisqxc.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gkxjeelxu.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gszxxpeqy.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gipsvbsdm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/geyhpcqpy.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gbqlenkzn.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gvmzcblqo.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gncqyckty.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gprlliwqb.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gumqxdqpw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gouuviung.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gucjyzcco.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gorsjlocy.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gjscvsqwl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gnbemqahp.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/glbtwauqx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/glfjpvobz.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gabomlowz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxncmcro.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/ggecepcye.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gabciinjd.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gznqjwnop.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gqsiiuoim.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/glspnsprj.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gctgqbtip.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gsocgdgpw.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gfqhqwcfd.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gprjxkuqs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gzevlteur.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gzhozhpza.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/grfhvbyeg.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gqenmxbnb.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gmrbyxlim.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/goxuwoejk.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gmffeesfy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gzyjfwvyh.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gpjrwlkdr.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gazffxcyz.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gpofixmts.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gvrvogccv.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gvsvhmcdb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gsvfwljrk.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gsmxoburt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gatmcyaus.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/genecprui.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxhxeauci.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/giraexzkv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gsbaxsjee.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gnqinxhdp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gvmftmaib.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gvrqqpivy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gwdzzitvv.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gkrfwxsff.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/goznpuije.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gmyhqjxho.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gtwpcdbdm.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gfyjscnkw.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gxxzlfzwp.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/giuskslos.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gxxrxfacx.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gcbhknyfk.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gpbnwbrdi.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gjskpythc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/ggoneeend.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gqhvmhokc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gmfjwvtyy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gvphqsqgt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/griallblb.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gggrgnubw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gxflwlitf.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gsmzmdebb.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/ggtxdfqhe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/ggiysubin.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gufucgcgn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gfkhzvsqi.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/godrqopwg.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gtqkxwanq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gxsxurzho.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gvvjyzkrm.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gxrwucfvr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/ghldaqpct.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gtkbajpqy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gqlefwxwb.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gdgyooack.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gqdqlvapw.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gxtwqhozc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gtzzamdlk.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/grfzmioun.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gkjvmmbvy.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gdueszsge.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gpcuaiser.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gatekkopy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gqmjzewoi.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gmkokfisu.sHtML


<!-- 参考信息 -->