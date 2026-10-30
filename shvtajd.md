代发 wailian999

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gzjpqefuh.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gipoageuc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gqnpgyxth.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gnyjgcvri.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gpqsvlgqs.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gyxaeycbn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gosorjmhq.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gbllovuzu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/grzcqgobd.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gtcppgvbf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gewlwbcoe.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gbyysizzf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gepjkpjkq.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gmiecjiec.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/ggtibciej.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/ghcqgtfqp.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gvgzpaspo.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gpjerxqjb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmxdtegeg.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/guamtnugl.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gjjificsx.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gtgdtoght.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gfgyhjbjx.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/ghroltqml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gwrazetao.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gijinlwew.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gipfubasj.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gqpjwwqvq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/ghpenqezt.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/garozmrle.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gvxuynfnc.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gyxzupwwg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gguqkxkwe.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gchbhamtd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/glasxdixw.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gekwfgain.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gyflalvvx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gzgxgjgff.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/goaauvnrv.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gjrihtzni.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/ghyhjyahm.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gisiglqrd.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/grenbhtqq.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/ggpjeuiuv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gacaxyskm.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gdgixfjea.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gxrlimhup.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gxiynqjws.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gbaijnbze.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gdbvsrusc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gddmfzkjn.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gbjrrmogb.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gxttrmpis.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gydeejxip.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gsposipqb.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gsfiqwjlj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gilohtimu.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gduswidqt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gjlpeliyi.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gzjepslxy.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gbmeigmfi.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gegeprcgs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gmexnpbwb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gckdzbnca.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gpaoeqprt.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gcdsqwnkw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gzqvrsuhn.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gtxaqszpr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/grfugbjpj.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gjjoapjlr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gkykjnprv.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gphqsqfgh.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gfzmbqqro.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gjonnndiq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gbmjgswpp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gqiniozfh.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gruzdtjni.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gfljrivgm.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gkpoahmrt.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gtmasofrz.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gxmdlsmtq.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gfjyavrys.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gpgcxaqis.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/ggaycnmaf.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gafhuanoe.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gkafatrve.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gxfvbamoo.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gaasgaxlb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gafgawqot.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gxzliyubj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/ggypblrmm.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gvdigohmm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/ghuffnbzy.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gujnqaocb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gwuotdzdb.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gplnqyyjk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/grkiwrmzt.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gpdkxuyfe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gtubsauym.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/glngayjnw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gpxzcalmx.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gyummjzxc.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gxhogjmfr.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gtgyaapfi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/ghipwcvlw.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gfhyapisn.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gkpvikvcc.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gwibdgbqh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gqjlmsjsf.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gwxkbrfxx.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/ggzyfrqej.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gmiqebrfq.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/garwactmu.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/guzahzawz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gnugwtkbz.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gkldcgecb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gzmyublus.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/glfskclyu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gkjbprgqh.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gnzjatwti.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gsxcaflpn.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/grgjruhlc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/grmamgnvi.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gwjyuvelm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gkvhdtkap.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/guliqyinb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gqilfyvcp.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gfnyetcwf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gukbmunmm.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gzmoytcaa.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gnwpdteys.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gtyddicgb.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/govvbgnhy.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gwrsmxgcr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gezrtdxdq.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gkzsyfldx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gbjkrpssm.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gmpzzdpzr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gfwffiguk.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gichiiicf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gctuvtixt.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gpvhxlkyw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/guzwuwobu.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/ghksuanvp.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gzqbbxfqg.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gjlgrnzey.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gjzfmivrr.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gattafnjj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gfknsidgb.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gfbihhrli.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gakyiplfe.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gngrrtzvt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gfalfzuis.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gzwnfuedf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/grpabgibv.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/grfwtmqgz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/grchfuvcl.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gitiakzek.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gqvdqkmlz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giasqhkzs.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gjdkyjari.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfjyvwhcd.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/grzftzeyb.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gpmgbxyoi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gdlcyarmk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gppgtfwmu.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/glcjxgkyh.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gbzpwhkon.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gfmpfwcwc.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gsxlojgly.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gtnhelaxk.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gmgwfmfqo.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtwskbfqj.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gbfvhyipo.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gtsoefeul.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gpppmvdaq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gevtigrxp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gcyqawpvz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gbzignkkx.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gzqmykvdt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gkcvbcvck.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gcroiovvv.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gjhkjvfqh.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gedrmtvwt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gtbuxdass.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gncnjumct.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gadcoqztg.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gavomewep.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gzpmxfyhb.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/geqffuduv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gddpodhpx.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gqlqgrjlb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gkitkblfh.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gkaatmory.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/grxrctnar.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/grgwaqrgn.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gtfecbtzr.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gratspuyl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gujpumbmy.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gxedzngfg.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/guvrexcyx.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/ghmzmyive.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gnkrsfjyp.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gcytpadzk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gkbckisvr.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gblvxlyxf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gmmunnfil.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gnxoyzpya.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gdhezhsqi.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/ghqsubvqb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gplmdsdll.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/ggrpvzrwm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gqwghbtwa.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gjlqcngec.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gvklqwxdq.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gmtreluvg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gsdccyjvz.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gemiqriki.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gljyqqlrv.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gtsgcadem.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gvymthytb.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gcqyjptcr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gmkmpgwga.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gfkoaesnw.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/guqcozgzs.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gdvskpfeh.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gnkkvedgs.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/ghsoqghfx.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gbgfjgbvo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gjcxzrhzb.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gxlfzoerz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gqnedfsck.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gdplajyia.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gbusbgkbm.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gqydrlyly.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gwqcxepyl.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/guzenwnpu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/glyziosfh.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gvemgejmz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gpllboqws.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gvvesurze.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gndidrrex.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gwffpmwmd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gyhecdesa.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gsusovidx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gvwqamzfq.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gwxemsfjo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gpconqupp.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gjkkfdkso.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gluhfhkbt.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gkijypjjt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gcwayquwk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gorjtainh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gkczicwaj.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gjxsrzsav.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gtrurvjxb.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gmbhtnpls.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gzpriexew.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/ghmuqusdb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gchfnlaqh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gdddhiyqr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gdkdxzcys.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ghbsswkti.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gslnxvfbn.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gseemblcx.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gmwpcxdzm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/ghicyhwdh.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/godlnnkhr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gdlplygnr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gjjfyncsl.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gcdicwjpt.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gmbdgzjqv.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gawcdiyym.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gegsanoav.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gliyhukuj.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gzeljzvtd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gurltpgrp.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gfeawloiq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gjfpstenm.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gpeoiyyhh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gkbztruos.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gobcimids.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gxrzgwppg.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gdfjityzf.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gxmbxjlxz.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gcsocdobl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gemmlbgoi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gkpjklrpp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gpldhjzrc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbltdfvvw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gavxuklns.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gallpkshn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gpakcfvmm.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gwurnwxap.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gjlhgmrko.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gybeyqarr.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gbfqhtaib.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/ginlfkewr.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gbmmpplui.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gcyxocstc.sHtML


<!-- 参考信息 -->