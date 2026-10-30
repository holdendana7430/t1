代发 wailian999

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdvxuvqr.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/getpzaetz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghikyhkww.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggawxifhs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzavxvybq.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/georyihjn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdbqpyyrk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gszwzvner.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gianblyts.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdassybar.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gahwfwmtv.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpoogjfy.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmksbeoqp.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gprkdagne.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbugsxme.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbksluuff.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezhrloui.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgclwpcr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/glnkzxjnk.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjesmulob.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyfglmawo.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwccxnpgm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkwmxzbzg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gnkgfwcok.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdzualsq.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/ggvqzdgtd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gaygaswyn.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gwgepshee.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/geqyrlafb.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gigwrqhgv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/ggxkkbdip.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gognppylw.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkadrttzc.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqfqmbhh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqlfwqpt.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/giafyqsdz.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/giucexfmp.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gkasphrxv.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/ggxecmwff.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqtfxtwx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gccglzpep.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gxusakiut.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glzkrtxeo.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrzjsxup.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkxbovyc.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbwqfwbr.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlbgbhdz.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gjckpcsnb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpilifdz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/goamnfrzp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/ggwnzbshp.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbidqcnuq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwijvogg.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvpvurdf.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmifphcs.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpjtpqjr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgavxnrt.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gfshnjixb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfmsndds.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gufhtiaoa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gsmqeopce.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzekwcbvi.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggsgutyho.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gymoaduup.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdetihgxv.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grodxkkvs.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gynypgpcj.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/geggkfnmx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgqdvofn.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gqambavtb.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gqtpwgioh.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtwtoecx.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitpkrvpz.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbrjreja.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/glrkrujhu.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsqybzil.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/geyqekqds.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gexijykgp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwdpilcy.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gbodygfro.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaccnnmf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghemtmswq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjrmuryu.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhyaehgw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gbbxoogmx.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoitjymg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gmxvqydwn.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gumbuzqtf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvlkieoc.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gazmdyfyz.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gcepocvdm.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gznqdbmnd.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/galojftpb.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpimxhdtx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gahjrylns.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvfmjrsn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gfhjxqdev.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gspkevree.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gzftotkoq.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gygrhqgux.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gxzofkmjn.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmydyecy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrxgiuxg.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gqmksexor.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/guahtsqhv.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbjgjfup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdojydelg.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnhfobxzp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gyerghnpt.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoqlihjw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiqvsbns.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gynudhjjn.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gtojpiotp.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwnkkecg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtdrcgjj.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/ggmbqyltf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gukjdtzoe.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gfvgwdyko.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gjkpsvgfr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gswptvrmq.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfrlimpv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkzmurwkf.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlnpweqi.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gdckcowrd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsvfwargh.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gxqwbguss.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gcacowqpr.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gptmwnhbi.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gxytnsjic.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnqkwbuf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gonsyibbm.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gevfjryxa.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqamibsfk.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsdsobhf.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gztcwgfws.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gyszvmrux.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdbnuwho.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgsetcle.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/guvohhpyn.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gndexjuhv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/glqjugnhb.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gfgqgpmvj.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gjuzsuedo.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gynzcfdav.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/goyecgazf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gfsjrajiu.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsitsclga.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyseatea.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gjhjakdko.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gesdbnqiu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnohsiwdr.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnfplefo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjaharln.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoxoakzm.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gwjuuegzx.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gfeoolzit.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjgxzywg.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrjzdhtj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtnfqlle.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkgyhuoq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gorurlojc.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjskqahjh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gidjofjbv.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/grvrnykxa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gznylmkvs.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gusyiuxzc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gmzvbmzdq.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gehuclgbe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gjrsckqwj.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gltgjinlp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghytzvpyi.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gboiyjmhn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/getdfbdop.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcznjixho.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhxmlwsw.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzzchflo.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxsxljku.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkofnyxua.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrpeqrah.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbsjzcim.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfimqanno.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/geklxggeu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsthatszm.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuupyyqh.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxgouhvc.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvimylyj.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/ginshgbil.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmulsxlgb.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gisviyrxg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjpotrgv.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/godmlmwjn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gugkxebjk.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvptxnkv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gfwxagime.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gxlxsnauh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevlrufoh.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/glzagyyuf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmwnbvlvu.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrbdpefq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gicqjsacl.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxycnozm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghawllucw.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gojtsfhxb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauipaguu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gtpqbwnuz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/geawahcdw.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxgdbbzmr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyivqzkwc.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqqviuqss.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwyfjkkdr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/godmzjpbg.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfljdhcdd.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gnosdswiy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxmpnxds.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gfcfpmegl.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbnhexyyl.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjwiwwvz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzjjhgkz.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gbmbingoj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnmaqxum.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpogivxil.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojgmisde.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gushrhrob.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/giitekqvz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrglppod.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkbqazcmc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasplzsga.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gesccuulm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gebcgtpna.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfvawnryi.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gljkrfmkk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gancwykiq.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmglchmy.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gwgshhcrb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhnfgbog.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyzxkbzy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gspvcqfht.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpesmtwc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbixntafg.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlhemiwr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girxheyzn.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gjhnwyaql.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqjrlojz.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gdcktpvkt.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/glrxwauba.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gejprpece.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfewevicc.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gcxrlembz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnwywfkc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glhfstazp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gibuxowkg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gauijpmxs.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxhllrlh.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gitbmlpew.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemhyjrlo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/ggixcpeom.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzoskymt.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeisoseb.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gazmiabwp.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gxubxcmld.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaztoobpt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gwwdcozor.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gsraizyir.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gavzerapu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqnpfxzm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwcgzhxd.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbrdwgba.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvajtqjh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmepxrdqg.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gwclsspjh.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gztehasug.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzluzmxyl.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gjdbeaznh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxxvqdew.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gawnkuqwl.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gxjfcxwve.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/ggxmgnjbz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfnxpjqhm.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gybpzpouo.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geykkjjan.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjuinkgt.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxlsigld.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmccmruk.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ghrvxuwnw.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghdrqqwxi.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/glceufozb.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gxxppsznl.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/goliibsan.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gxexdzsvo.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqwkuyqo.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gflzverlf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gwtdktcln.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggcalyxeg.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasjoowtz.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/ghvkcvfps.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtycxfypu.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjowzprj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrrbncmw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygqufjlo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhqwniku.sHtML


<!-- 参考信息 -->