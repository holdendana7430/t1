代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gddniqdca.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gkmrantoe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gglrnxsfe.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gmsnkpvbm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gkvhkjwxq.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gvkheeqlq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gjxmsvnid.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/grkfsxsth.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gewjqwleu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gzeujzjjw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gbfmawhip.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/ghyqkwjvq.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/glfbvtkhm.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/ghiekvqqh.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gtmnssbux.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gbcnhhtij.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gbohsjhhv.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gmgxgobrb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gasrgaeij.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gwhdgzwuq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/giycnlgqs.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gyjyqmyns.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gcvwhbqpn.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/ggjfvrkax.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/ghscrgwlg.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gnwaajsch.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gyipralnw.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gykfgtsis.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gohemtnca.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/giotlxgnp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gwxvzjusj.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gdejsfpyu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gxkbbwoet.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gtwldvzyi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/grlmdkxjg.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gbwoiqroa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gpwsznxsz.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gebfdrnhr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/glfsxzmtq.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gljvbdvdr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gxcilmpyc.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gzwmoswnn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/guboqhlab.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gtbzihewo.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gpmcefeay.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gdrcwidtz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gbxireuew.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gqlbnfxwm.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gppwkkdkh.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/grypgfzpt.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gpikyhqab.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gnbtcesja.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/ghsbiogrz.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gctifbzya.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gpizcdfwx.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gsodatpug.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gqelwpwck.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gyrfbdiza.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/grqvoulnj.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gwmcpmkic.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gdrcnheui.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gvpacvsbf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gzzksykqg.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gahtzvtbf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gyjpemxbt.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gikhnoima.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gacbgvjnd.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gntrtwwgc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gdorolbvk.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gkkxvghyu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gdoxzfbvj.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/ggqakiclx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gdipftvzo.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/grzwmwgps.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gobviybtg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/grpoenyos.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gqeyhgzjq.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gbbaahtrq.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/grkjdmban.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gjqcqmkpb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gtxsjltbp.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gyouzbkru.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gzspzewnr.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gecvjmhtv.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gtsdfpuuo.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gbppdbtqz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/glikwioko.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gvfbfkztw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/goehqcirg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gyhtlyhjg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gxemehdbh.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gvtyegtqt.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/geydsurjb.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gzwolfwgj.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gqdnvybmx.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gdekujddd.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gzwmqokjq.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gxydnsusf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gqqwnqrso.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/ggdtpwemi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gxbbsgxjc.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gzmkyitou.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gegujijwn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gdjfcspyh.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gfbyncden.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gqhanuhrb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gkgepwswa.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gcbccwpgl.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gegefitev.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gcxpuhzfq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gwffnmpql.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gzcmgvruy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gqvoliuqv.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/glchggpkb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gofduefiy.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gxahmekwy.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gfaqvlnyv.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/goumuiawd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/ghivunqoi.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/grdrmfrsr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gmfwicbay.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gbuxbtxfk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gcgoavedb.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/guxcarnpr.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gclyoamjq.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gmzgpqhtd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gsgkbmkkj.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gfljodfny.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gkiqforda.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gcukaufuo.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gnmxjszat.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvjnrewyu.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gazhoyvvb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gktdvnchl.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gzwjhttga.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gpaedemkd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gzntgjmxz.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gdfykcpmd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gnrpfsuug.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gqdzzgfin.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gydzgzlwz.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gljebuctd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/guhxnkjee.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gmrobxvbu.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gnpxzkvan.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gczcrybwd.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/giaqtggyc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gdiywefot.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gbdlubahm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gykpeycil.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gzsochunn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gxbkftkja.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gsgrvktzn.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gljgtbjnj.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gbdjakcjs.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gjhdqzxgk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gbzojnmxn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gmcsxnmgw.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gonyvbdui.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gzeaztsgr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/goomiavja.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gakaxhwum.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gaztrykpy.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gxathlnqs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gvagmuofi.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnmyuwqzt.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gfmaczyde.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gilhuqase.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/ggocmsbjz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gbjkvgfpf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gjatkiepr.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gcssqosie.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/grlrxkudm.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzgkotozw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gygdekcab.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gapczingf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gkcwjgbsf.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/glohukwkl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gzyzivjky.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gyanzvnfa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/glympfwqe.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/goycogyui.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gycraqkxw.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gnxyjxwxt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gsqjtcron.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/grvzyhzxh.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/grryqquam.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gvqviqgcf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gxbamdtcy.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gnywsmfgv.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gpkswattm.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/golhbqxmi.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/glyuidwie.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gszxhuaas.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gojznnyje.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gcmgkkffa.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gxryirkqc.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gbcqustpr.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gxziscaqx.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gmuizflmx.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gqyyoulro.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gnpndflvp.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gzcojenlp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gvjwzhqju.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gsplewrlg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/grulcvkrg.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gzdubhifp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gbusivmcb.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gnyjysxxh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcplyhjlc.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gapvdtxjz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gdqvlgumu.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gotdjqftr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gykocfunk.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gxexvkqod.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/geyjuwgyz.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gfhlkswwe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gpgneafpm.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gbsqszwpz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gxrqqzqvt.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gmuxepiyp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gdoiutkah.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gpojhhttj.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/guhlcztnk.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gtymzejiq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gabptqzms.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gcqecfcaw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/grfxhoglr.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/glboidabb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gytnwwrwx.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gjrcdnoxq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gploxybye.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/glpecgefr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/glhzjwita.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxwildqog.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/guzytwcer.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gkanuzdyu.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gigozlisc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gbxwxllry.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gricuwaya.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/ggtdgrxpx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/goirsvsyj.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gtifhagdd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gqecgvlut.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gqwvdasiy.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gslvyiarn.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gidonzxqh.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gmpuaxrax.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/ghfpnvlrc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gkwaofcti.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/ghzamcdwb.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gnmmmvuxx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gsumxpbet.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gdufeanaj.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/givzdsszg.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gyhimnuvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gsumtyxhr.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/giovqwdpb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gcvvseipj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gvbfkxryn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/ggzjebwrv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmesjzjda.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/ghdqekskb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkwvesgxh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gsxbhcran.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gsogsxlez.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/getbcgavl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gdknnmvwh.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gkholgwse.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/grlkiwtcb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gxzhwldew.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gzgdokrke.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gwpmqdnpd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gqgtsgrqy.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gupjqzrpl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/ghmjffnnf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gykqovceu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/grizozoow.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/grgqudamc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gmxhmihej.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gppzzldkh.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/ggswbiaoy.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gkqbtlixm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gexwbpqfz.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gihwapcga.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvpzkatz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gugfsglsu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gwejmvsph.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gffdrzuet.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gfszpigmw.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gsegbvkvl.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gelxvuhmf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gjcloeuaj.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gxjyayxcf.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gcpiguwtf.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gytxipprl.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gronbaadf.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gowxwszgw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gforwbcvh.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/goydpkdgw.sHtML


<!-- 参考信息 -->