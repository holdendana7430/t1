代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxrqpeio.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/glbkkmyfp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdoxbecy.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnhjnwllj.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfscfgsrt.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gozdauuqd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrlgaude.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdmanquh.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudgbngyw.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gjihnplah.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkidipfc.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfldxlwxg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggziwceya.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gddcoxrfh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzzrzldwq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gccmumjes.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjeyofowg.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvsgjxlyg.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gycxtgltu.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gnbwicpci.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gylpnvlhr.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gwatzmiqn.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/glrzbbcqu.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqsioact.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmbywdpdy.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gbqkvopxa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/glqlzxgqw.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxqmyjswv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztawkyak.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvegupoo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gantkeinl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgteuzie.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnngepve.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnzgvzcn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdehqpbg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwqujbsq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxbpomta.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gsjpwfgtf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gsanquxxk.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/guyaujkgd.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjnhgcoo.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttnxgdbo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gdkdrdiit.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gvralwryg.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjsiqxty.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gumsnqkic.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvsfpgga.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gvkeyjflj.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gkuzrjura.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeatacoh.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknzpncxx.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gclhxxabl.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdhmxznr.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbfofskq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrsppgdf.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gemzmobis.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxuwural.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gtklxdfjy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gfqbczgxe.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gstmkgjjd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghzblanpc.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/giqcvdtgw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grituoynu.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gogcvbrjx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gihzchdea.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gcfzvsgub.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtwrhpxo.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gipbsqmpg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gttyoiibj.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guogbgjkn.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gabnahsmg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwfdnlcl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gubvxfpkt.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmngescui.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnjttbhah.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgenxtjj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gytzrlhdm.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnewfdbh.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlblgafw.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzglhorc.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gmguqhqit.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgmvvmkz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtloyeydw.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnbbucjy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsmldrdw.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/giqxfvorr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhnemtym.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/ggvntewpq.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/guykadwty.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggajndqoc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gquyecokw.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyolzpvn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/glehkaqym.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghihfhboj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhcfzhel.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwugblvb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gsnhpxopa.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/giweyzdmn.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxfemjny.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gusomwikn.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/grtuvjwvq.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gohewrzfo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnggsrww.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwiymfpw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/giwxgwily.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gddykyzps.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/ghwlyagnv.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gdwcziviz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gxliirkgn.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrqfqtvo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grbjpemaq.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshtetdia.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/grmplcpbm.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gbomfzzxu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvulbulbq.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqvczpxfu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkadpuuoq.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfzmxpww.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwviqazrg.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gtbmifvof.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjsfrrad.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxfxekvj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gaasaordz.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/glkxonsmz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghocqbijh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gnconulbq.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gkjgxamip.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcnahvdy.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gvzqblash.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grqchtzhw.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpmlfpqu.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gcasbkvon.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrbesvxz.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gvcorsxjb.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gpnbbvluy.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdwmcvyv.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gqxjoihxc.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/godnbhptd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvemrzbye.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghvyqahdt.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gyyhuhjhn.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gbzwdgqyg.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gpkjpdere.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gmqnubsdk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gkxnjuaww.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gdwalygfq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhkjourt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsfbzkmo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gurilfhzc.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gwibwqruw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhypmvss.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gaojnvudv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/ghdazfjtr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsttyirm.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdealdbm.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcjesmysl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gpljdbutw.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvttfcijs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gvdmhkxmt.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gwqvqstqq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsirmpxos.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/glutbbmgf.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ghguwiief.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfkiouyb.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gttxhjofi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gvfauxtpy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/glzuvyyan.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjvuxnamx.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gounmkbpx.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxzmbvorw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gepeyqpok.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtshfzyit.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gilgqblqb.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gzpuoteso.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gggnnvvtm.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gylxxjron.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gxnfrwbzs.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmfwzomt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gddvnjkkg.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/girfccths.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gokqqtqzl.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gbodhtikc.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/ghpvzdrkn.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gaedwrpns.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galqqahno.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdawzclvl.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gijwpebji.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcafbwbh.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gihmfbttt.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwbrjxyr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxxpdwhj.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gxdtleebj.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlsxgtdj.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghradvxyk.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gmsofbzcq.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmcrsgqy.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsrbayij.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfhbkynuv.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdlpzonkt.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gutejracq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulsnyysc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ggzeahrwl.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoodtrls.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/golromyzp.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjdayrhe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdyfkuzo.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gagknrsuc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwljyfviz.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gfpwhqroa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghroysalh.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaxexohz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ggisfmfdj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgtrajut.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdjdpacp.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptfghghi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvfhbhoy.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gonqebrin.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gczoauxkn.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaiqsmafh.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gvefukevp.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gmskfhsuo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gicedmmmm.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiojckce.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxapblrqj.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/guvrsfeah.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gpuoekmfz.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gcccqxmtx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkoetbsu.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbquabcn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfsktzbz.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmnqhwcf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gjpedltjq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gypgnurbm.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdghegqqx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gnhyxzuxq.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gjuumymqa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gitfsytpj.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gahbifsjh.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geikruwuf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxobexloh.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/grzfbqwxc.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gzvheonzm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzexcsfze.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxdxacbc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzatkwrqf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gticwtcik.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaoywwbk.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gqzrgcpex.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gptnitdtq.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuhpblvx.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsunxzpm.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gcljqlyun.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwtqwauw.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/girildvqp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gymkyumcx.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgvuukoi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnxsvcjb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gticwgdmc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gvjpwoleq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdvtogzn.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtvgljltq.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/geursthzw.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnobukip.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfehpboat.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gakyujujc.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjsrgwqa.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gqybsmanh.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gdbeumaqk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gzvojskup.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givfjmzuw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmpjeply.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gfslewzbn.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmkeiszy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdulwilog.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/garugrpkq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gpfbycjsl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbldhufp.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gazcazofy.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gumjlmakm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaodyilyu.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gehkljrwa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiyykgig.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclwxacgp.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gjemhfmtu.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gcaaromdm.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gydmtszcj.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gggnvddnx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsadimdzq.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/ghproohch.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnvicyww.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsddhzonm.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmdzxipj.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gogydzgui.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjqcyiji.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/glxomazmf.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbprfwzog.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gzlsjksty.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbiglsnp.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkqhyyec.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gwdmamvza.sHtML


<!-- 参考信息 -->