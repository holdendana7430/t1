代发 wailian999

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gpxlbisej.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjufpwar.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmztitatk.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbemlqpux.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/grjnmwuqq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvcobika.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeuhkgfs.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvyrbaxb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdubfwen.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ggmttafme.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gsuikfvyj.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gblwaulwh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfplmfrv.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gipuhodhf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gqznjwzxx.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicjksqvz.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaicstyew.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghocdexup.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gesvsqmvm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnfkycsf.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gncpnykkk.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvfxnmmph.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlhaqabe.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgpjbady.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkiupcnme.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gnvkaoxqz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuxbeehb.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gggrhoooa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqjqmvtfv.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gpgdfohup.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/glrpdmbuq.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gfobbnsgq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliwjmvzw.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gpzunidiy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmbfyjrk.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gncfvavzr.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdypfaqzx.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvflnulid.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gioxkewtv.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxolabfk.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvubwdte.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gnivxmocj.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtxivckoo.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyqnvcrq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkhlmwnsa.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/govfxvcra.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsqtxjmg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhgughhz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxczoarh.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/goaazivma.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gxjfqifso.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gpusyayso.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gqbubcnqv.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvscdcrt.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmjzlcir.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyisnedgv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyzhkgpc.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/guijxpbbx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gngesakwh.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gthberhzs.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdksfemxe.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gnyazwmix.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaumtmijf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/giqxcjoaf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gpbmhxjdy.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjuydkse.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/guphhseay.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlhewspk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/grynyllqm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhhbsyou.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gekfspvrp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozglvhgc.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/goatcrbur.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsrkefqa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/goidtambk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gilzeojil.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/grpakxbth.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjahrsyk.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/glfqeazez.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glolpzeml.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpabnekpj.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/glwebefnk.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gleuwrojn.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbalauhmp.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gltwrjoyn.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gyemytjln.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/glhjriwbn.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaasmmfs.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/giznpyocb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gmymesmls.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvlhvzak.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmieyubc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyqrdyjlu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuolvdjf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqiqdxolt.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/guhxuyzcf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gvgtpvcqh.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqaermob.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyekgwayd.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gjdjegfom.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gyzrqskbp.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbpdbvlt.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gajfafnyg.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/grjawsaex.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gqslvcscy.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoojimik.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggjauqlid.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gupwlgqsj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcsjohmy.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/ggesbpplc.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggycbsenu.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyfgjkzo.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvmobvbs.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgcphghv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwysbzdu.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gqikuwhfa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gxizwbwqv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/guueasjqk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxgilott.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbburowb.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuoqmqsm.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gykzczurq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/glctkmtrr.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkjlwurs.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/ggvpedcfr.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gfhriutct.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhegnoaw.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpurxbxl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybaisook.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsevjoddh.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giawuettu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gekjtchgz.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gzwwgbkgx.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gtmqyjpvq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjuqxecop.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gfwtajauh.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gxuhhekws.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlsxyhpy.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gzanbvvyr.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gwsxamiuo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgmnvfcs.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkzptngb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzumjpehb.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfqdyzmcm.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/givdvhbdi.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gseypkvfi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnrfaygl.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdepyikp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoqgfxvg.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvpneqbs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrqesdnw.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gboopkyng.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqkpqlkt.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/guwuhqrav.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsmxwivoy.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvedwgff.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guabbanbx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/givtrjeqg.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqecttip.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxdfzcxq.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gybnqukem.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goedpgunc.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glbrravod.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gvfdizcgb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gztsutlip.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gyyenrfby.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gwiampxji.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/ganzcijnd.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/giddharwb.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvoxuskv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzieijwhj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjfejjst.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxprsciyz.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gwglhdjhi.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrlhsmqz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gkggscrix.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gcjoyxtgc.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrcjjhwv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gowbjhsuj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/ghrmewfug.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gctbetabl.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gyixfipqz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxyrrqyn.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtjaqufu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gwxogjsjo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqndcvsqa.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goofazwbj.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfgfkrusg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ggjpzetny.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gctzciepi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/grilbwnjs.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/golfimvhl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gswjmefko.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyhmbppe.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gvibeltud.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/grvlryctm.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyqrwtof.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/grgprbwjy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/guwdjzgrk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjtotypk.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gazoboqcd.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gawneufea.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyubnsegb.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gitbnxvtb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbgzyylp.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvbqxomm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlimoktx.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/giwzthbzv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gqxvpusvx.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyvalbxg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gzyfzlnax.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/glqlkxhum.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gelqbynqp.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gpjibcqph.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gebxvjfmj.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gbyfjfnpl.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsppccewc.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyvadjls.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkgndpxm.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdufzevoj.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gwjzmkftp.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqgivauzz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmvyghqw.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufardytc.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gklriqstu.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaqajina.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gbgsnjgbe.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcqparagp.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtwsszga.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfbvkgmgv.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdjqcbnk.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gseygtllj.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gnsdzmnhp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gszrvovkt.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/guckfculn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfyesyiy.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gnokrvlxv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnconbdqk.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gonuwakmf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqgcttez.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmnoyxpr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqazvrroa.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjevsbpv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/goteaxrfz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/goobztfju.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsyqbwgz.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/guximsvtr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gstxetiki.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsibwjoof.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gjqhsvkvm.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gugcesoqx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcqmihwb.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gafewmbdy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glluvxght.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/ggioydnks.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyaalljg.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzkyqtia.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhqwrqmw.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfozhsqg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzswbzeft.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/guojjenpw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjxpnertu.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfosrymba.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmedvxkt.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gvtjqbeyc.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gactellar.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvzmyzqt.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjjgsjzzd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/guyebsucp.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gafwpbpvi.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gmyvtkvjh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gukuzckop.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmhesgqy.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/golyyyuzd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknxyvoqs.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdxtarps.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gubzhwbgy.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/grhbdqgdd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gamebxbnb.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/grestdldg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxncrnavh.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gaypmrzyi.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqkvhbld.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxseqybj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gfaaujfab.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gbbrsaeiq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqrsrnue.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/guprafmpo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gdwraxxkm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glzbanytd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpblltfd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxtdqziz.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtepvhthw.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ghopenypo.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnrgvyms.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsmxcpue.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokfritfn.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktebgjgw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gulnncrfc.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gaabpxnbm.sHtML


<!-- 参考信息 -->