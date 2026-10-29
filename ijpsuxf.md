代发 wailian999

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gykcxfomd.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gqywrdxvq.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gnlnxvdpc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gokwarzct.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/ghgniqlql.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gixybqdat.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gcaguqpre.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gdgxfgudj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbamtyouv.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gnxtuhjjj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gjfbdqkag.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gfbylnmau.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gdywbnvgk.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gercpumgd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gjseedfuc.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gblkpsbbq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gvdoapnwb.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gbrkxjuda.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gsifnqblu.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gygxzoqos.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gzahigfgi.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gdtnzfhki.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gostbqzgb.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/graccrpks.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gberxhhli.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/ghzyujldt.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gkcnlnabs.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gditaecia.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gpetoroxu.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gciccwauv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gikcswuun.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gvqsmzslp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gfsnqygtz.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gaaculhwe.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gmyaplzxz.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/ghggijgbl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gxepsbxzl.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/glrgcpjdn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gwicyxnhr.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gqyrwwepw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gjhqnwgzr.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/grpdbokzw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/galdtprlm.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gjagwzszp.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/goshznotx.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gyximieqq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gxndauisd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gufbsfcgb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gkhsshxjd.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gckwoqnwo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gynkggbvn.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gujtmaxeu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gvbomjhlf.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gxhzwbvfe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/grxcjypcm.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gstoldbea.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gwsgsbqpg.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gijzvicza.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gobiheijf.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/grlwmitte.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gjlesjche.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gsbdyxpdz.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gjcwblecg.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gdteazoun.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gmlsevwra.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gvildswle.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gywrilgoo.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gfogqqfas.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gcnkwnpyt.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gjxjubjsl.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gzhkwwbgk.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gjqqqvder.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gjhcvbvka.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gbjgtegiw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gctncbfla.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gmwdytszg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gczhfgbbs.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gtpfodcdp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxjqurgjb.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/goaimmbvj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gizlszjgd.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gdtjoutia.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gdpedfihu.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/guiiukwcl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gmuzpgyyz.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gigxbwybn.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gliaidezx.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gwzpzdcnj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/ghycxpdzy.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gxbaxjocx.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gxiogjshi.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gzdktgjsj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gclfxtwmb.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/goytabtve.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/ghuwhatde.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gunrwvfsd.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/giwziamjc.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gdrgmfrkw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gixqgtkku.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gnqxqmftf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gxsdiefzp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gfljpwerk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gmgzlohuu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gkhfygnhv.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gdkpxkgdv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gkxftneyu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/ginflvzit.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gxbswqehq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gendfzjro.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/genbcgxle.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gztlurlkn.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gfuskwhvp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gqkpftvri.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gfahtoquv.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gixnzxpxp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gftjctzmf.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/ggesgglbo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gsamrplkd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gmntznaor.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gbeupgrnd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gudegpvel.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gfwuvilyd.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/ghynaogcv.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gfrziqehg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gnkxrxhvf.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gkmjefefe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gobbrhcho.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/grcntblyt.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gnavsobkp.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gkqzrbtha.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gatrgapmd.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gffujetha.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gwsriiwmr.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gtmgymsff.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/grxynoyhz.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gexishujs.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gotwzwrbf.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gpxyeyuys.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gpgipnsau.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gkivrgvph.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gakpbwokh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gmjwbyckt.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gsvqzzhkb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grsdemuvl.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/ggmkxwgsg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/govyodprp.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxnfxeqkd.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gtcrlxkid.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gmbqphosz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/grxykulqg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gyvxvistn.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/ggfziuzwb.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gbqcmttla.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gpfugndrl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gvevlvdsp.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gyqifdmlk.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gbxnmwvwo.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gqbpcuiyq.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gjkaddesc.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gksvkpsnq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gonsheugu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gqqvtzncf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gyvpyhhpr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gksuydjdp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gswwlmvax.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gvmqibfmx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gwjdypagd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gbqqzxnuf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gqfuflovx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gthixgqeh.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/glolsnejg.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gbcgvuaky.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gvankinhn.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gvvscwahq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gowexcgsz.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gghrkauml.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gtonoctxl.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gwdfispxr.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gdglxwxmb.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gjuaistlu.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gvilnppzf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/grprqdclq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gbfpikgyb.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gxnvzlfhd.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gzxpinpjp.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gfmywqixi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gaswikcdx.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gaffcsrkw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gpfqgqzkn.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gexuytcnw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gdmtjfgil.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gdedellra.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gxmnqjppi.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gigxzbaus.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/ggyrvldes.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/ggyctkhxv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gnxjbcyfc.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gukbnkxpi.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gozjpzxad.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gfetjhydj.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gnobgykdz.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gxwkcuyte.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gclzlfgci.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gkvsyilyl.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gjcxwrvhp.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gsvlkjcup.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gaujuceem.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gbztiselx.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gnsukmqxy.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gnbbkhona.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gkstvrrtu.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxmtrksqc.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/ghrbhdgbw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gnoeykbch.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gaeuxqzbi.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gaedrnpfk.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gdnwodjng.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gnsqghtst.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gwedzailm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gixwclmvs.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gabgkibgk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/goxmweiab.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gmecgfsij.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gehprmowa.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gdrfagdzo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gncedwbjh.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gdgttfkwu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gesmzklpb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gtddrvdma.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gzqikfdyq.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gtunrdkqj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gabiyzztn.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gpsouyppw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gdmrthbsm.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gjdurwutk.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gtskfhree.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gbwseoysc.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gsttwxqli.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gmsynzdpk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gbubncsyy.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gerguflfk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gyvgewuug.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gthbhhwyi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gxrceyyfj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvxldesne.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfwznuzhy.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/grohsdygy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/ggmchgsgk.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/geopfiezm.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gxgcfwtyw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/ghzpcwxxs.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gbkyqwxcu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ggftzeodk.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gwrhglmca.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gviwversp.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gstqzrcit.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gixkhngmc.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gyophzqmt.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gsjpyjwpx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/glyrsjtwk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gyvcirymz.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gyyldbbab.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gshocjtsu.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/grzwepzvs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gtavcjrzj.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gmsnbbabu.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gltadnalx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gbwswyrjt.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gxifozlzq.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gvkrejkgh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gdgjfpgps.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gbnwsycig.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gdvhulthh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geqljfgtt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gvbrwecni.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfqffedzy.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/ggbounfzh.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gmcaerfyu.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/guixvniuc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gxedtvfzl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/ggwfuoadp.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gblvxsoex.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gbuxjdjun.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gmcufomlp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gqfiabhng.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gmkzsqbyt.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gvtrinmag.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gooihjgbo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gorqzfaev.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/goxajdsqf.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gelooqowc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/glkredwej.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gmqlndgpz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gijwfretx.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gxuqvouao.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gaiivoqjk.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gotmagvgl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gwfknbfqj.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gzwilycaf.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gmwhratlp.sHtML


<!-- 参考信息 -->