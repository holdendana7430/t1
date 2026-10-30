代发 wailian999

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiggaqrf.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzglzqnc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/geamglsfx.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gvcbzmvac.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggegqgpzu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gznjztdan.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gynhunhku.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqnrioxky.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcaowqkz.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjdkuzyw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtfkolzn.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gktijsedd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbucwsttw.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gwyjfwakf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/glzldfsqc.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggasffnku.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkgbpxrg.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/giuqktqdh.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdfdhxfv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrvjpkil.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/ggevvqmrt.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gimbwiauv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grjkqautw.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gkzglzvzr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdazvacxv.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gcvtmbvix.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gauqgxcbo.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gutsybdhn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrlfyndy.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmscbdyxs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsdmdhyn.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gsfonjrbj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gegfidgyk.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpthijya.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/givkfrcsh.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvtsmefuo.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrqtshvc.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gdsirxkqo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmmpyhsqu.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjwypwvb.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupqqymas.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmvhnlzv.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/guotwjxyy.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/glrcpfvpu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gisfugjxc.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gliyqzhtw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplcimgto.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkmfhexl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqairsxhe.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyaivjysp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzldslaxn.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gupjdecco.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzhmojyx.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gnocdgzja.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gyucksqcx.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gltkdygbf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdnlfhac.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gskidgqwn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaulzpyl.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnappuesm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtpxxxcd.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gyipwqkbw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gniswzpws.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjeookxus.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gmbkxvric.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfmempuu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwixpujld.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gopulvkio.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gfkbbcwna.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gyxcmowkt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/giwzsgfxs.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkixqoesv.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnozirorw.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/glvkgusad.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gcpybbtyg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghypmvvjr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcbcecxp.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gqidnaexa.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gbjwfchmz.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gvfcqsccz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gctizflkq.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjxoxone.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnpfbhkxe.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghacsfqff.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gvrgyjdso.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gaashtiwo.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gbzfdqeuh.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdbezeva.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gxxpsiepk.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gynwntgiy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvpkuwjx.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gcpmyzfjn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkhdftdtq.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfwcqsus.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabrqiaww.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/grgxkocwx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqrbdjdw.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnlipoca.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gicloklvp.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gpvvuvrot.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/grxsjpmwl.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gxcanfomb.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgwtlztb.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcyzebzk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaygsxlti.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggwtkltap.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbldxpoku.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfeeuzly.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhodydaq.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdtosfeca.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqqbdnoa.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvwcptvg.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gunauvmll.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdjaaegn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqpiayrx.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttirbrlj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqupoxuw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbhoconb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfwpfnmy.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/goooqtuat.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjvsuqei.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmsvsytca.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjagsqra.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztrunlpo.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gsrvnhtjx.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtalcuxex.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gxkdtcsyp.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gieibpkla.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdltyrpky.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gpdlvmcba.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeppwygy.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guviejumq.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gdmqrbmxb.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrrfcmzx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/goovxtyza.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbewrtoy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gyornztyd.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gpaybcpow.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gaivvlxho.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gcplwsumh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/glcbjovyg.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gxejdtdmy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnzzhjmm.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvokrpiwl.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/giczgphpg.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gcserwgdy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbluhujb.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpttvzmws.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhcceivo.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjlkxbeql.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gfayukrtd.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gawocnuhb.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gzlmiacfd.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfesafnm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhygpkfc.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgcqsizd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdxtdzdd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gwewuphds.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gbjoonknl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grrvnlsax.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gdctbovfx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gngeglbue.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjesephd.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/glagcwupe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grgebynxc.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbtgkdsc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnxwogup.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gjhzzrbzv.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcpnxuvy.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gfgybvssk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/glljadule.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gkpzlppge.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdfmmqku.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gnrwuyshy.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvfnjndt.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbssbinv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxijyzdd.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gbqhgaoxg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gybodnzkh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsnzlzde.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/grzncmfne.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlbufbbf.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gaqepfgki.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gurjbrhct.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/ggybuscte.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqzkgtij.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ggxwfusar.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxcojybk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gtrxgtlth.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gbseellmj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvakhsbr.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkuuhyjn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gchfvrbtq.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gvbzkyvao.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gukfyivhk.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzwcqoeo.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwpkkbys.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grfocicre.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfgjgxhq.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrtyeylg.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpsypjas.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwvjcjme.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/goupoeugk.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpesidkx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gydksgspq.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gsikkshft.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gtezptjah.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjitvnqx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/goeeumesv.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzykflhps.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gbitcwftn.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gtexdiwtm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/grtsxozpr.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjfnipin.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gmbmycpav.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gsclifhcz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gekgbctyf.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gybbqsfjz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvunhbfu.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbswcsha.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gcfbmndpo.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmvhizkr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gamhjfgsn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemxjpwfx.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gnadehudq.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjwuwhsg.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjrplnxc.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcugxxfy.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxlebgkx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcvwttix.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gkjywjgrb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gbejbvfep.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsamhikt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/glccemskc.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gibqjxtkx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzogtpbre.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkasjxpni.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/geozzxzxq.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpkqlpbo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqztfojnl.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gltfkffip.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goydvnxcq.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfsiaopvt.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlzthxot.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugqxruw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxncysjy.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gzsrymsdk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/guvgrribr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahoegfmr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gbajdgodb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gutwpubdb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiymhayg.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacqnyoqh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gpewcqyvw.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gxxoivpah.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gddhtyixu.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gpukqwcml.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/geievehoe.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gnplkydbs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrjafbyv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gawlxcskj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpbsifscx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbzxmyza.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gktvhomqd.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gachtxptb.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzhpowgi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaksptuh.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/golvxbowv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gxougjweq.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwfcbvtpj.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gkvnnzlyx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexaptsxv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrmjbxnf.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gzszeyfba.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgslcxsm.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gtgkzijor.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/geofmibcv.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gvamhmrbn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/goedcmnir.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/ggiqbdeuu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqtfnjip.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnglmunie.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gjxezjqvm.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkleitoau.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gxhpbbpnl.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gnbcjcmrv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxhnstzg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gijvuyffl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gfnjyqmye.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbfvjvrvu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glepyeetb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnahtjiuc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtqdiddc.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdocvihy.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/glaaoztdb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/grfsnnqft.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gdrfufreo.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gictzelms.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gglthfjrw.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakubkahc.sHtML


<!-- 参考信息 -->