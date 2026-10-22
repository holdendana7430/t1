代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ggfcmzfk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bnobwxtq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cbmdkjlh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yuevufau.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2drphdxeo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2elfmxkal.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ezwnjsym.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2fidjrbxa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2khyepjej.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ryogjpbo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cgttyjaj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ebtcbmhk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wppjollu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2znjvovum.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tvliopqx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nurwrmgj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nmfhdxmd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kbzbworu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2auhumxkf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2manrkgxm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xrmexybs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jlsjkzxe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ccutpwoi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2aabosvfq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2kfgomnys.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gxrmaxee.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2uoqmkxlk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2swvufxhx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gdtcncrj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xzyoxvlt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kwqtjndl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2igcgahcc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2epbggxyj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aoymlmao.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ewfizhro.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fzsoasnr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycxjxuse.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2txrbioux.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xsvcimfj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2btcxhztd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jwpmzmbf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2iuiihmah.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2chmzgatk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2japnhmaa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2yufsspvp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dxeyzuoq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2lvzmstyi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xmdipgpw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjalbjrh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ascvrvwu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dfniksad.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xnilmxuj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mqweyzzt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rkticcxt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wtwoyjkt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2okkvgcxz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pdqsugky.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2humducwn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ygbeulsm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qiwzvxcf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2shijkvns.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zzxkpeey.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2dycjduwe.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2udgsqgdu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2lqlzpqjb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2pbgpntuq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sjayytus.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yhygwzne.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jqrphjoi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bnattjwr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pzwgdcso.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2aqjcwvfg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2whpbkjvv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zaqhzrwl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yjswacgl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2swjcfvsw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fgmcclvb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mbhiahtz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ogjjguxj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vxhuenzt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2waysljio.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2oznoxzew.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2blasdozt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ykmahutl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mywcchye.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ubxaepqk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xzwopemz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mldbbmco.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hjnhwglw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zcvrwdux.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ozzeglls.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2akhvcvcs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ubdzuems.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ujofnkns.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hisamuum.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zmdsyavy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ufuahfje.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2fmcqcudl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bcqdewnh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2lhnpzrmn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ihzbonky.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2olzpjwwu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rykggfrm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zxrxbqvo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2pveglwfs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dsfgysal.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yctgavuk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cpnyumiz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mlgevmpj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rrtvpeuq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xwcpjbga.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2uwdpkzsc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oufijhco.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2unfymepx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2lgkbqbos.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sobyzxza.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2doptyxgc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ozsdvglw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sbzvqzyr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wvtgbmlo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qzfldipr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fvwvseyz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sahpmhan.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dvmalwnt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2hdjzrrus.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2argmdhck.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ngxuubyi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ehtvsbbi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2doivmtcw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cdevjulx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ecqkeisd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tcpbdwwy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ckivpanw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hihskxvx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zhyczpkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xaglhqyy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ymyasonq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfulnjqb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2swlpfmad.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mqbntwks.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wqwihxel.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qfwwdsxl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mnzrcvzy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tmhmrwpg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jwjcmxyt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2fqkblnek.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mdopxuxu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fgrqpyug.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sepiwnpr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cqwkrfrn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2foxvruxb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ackyvzty.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2uedqhzxr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ojoesbka.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wfqyocpv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ivsfdgtr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2cftezvmf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gldxdlft.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwexhp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vpuazpna.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zoyunyjk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uspkdenc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vfokagnr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fkzkltjx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rkwtrjug.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2lvhsuzoz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bzlqxsfp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xrendxli.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2uhoejpxd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gojixaaz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qykawanw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2izejynjl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lvhyzfzi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dudgevzw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hfzdwgvp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uvguktmq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2cucaynwq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2epugkjlz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hciwosqu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2onygkrcf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2amwzozmb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wfzifhyf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2avwjoxay.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sgxfixuv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2pcpxecmx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2bbhxlgxr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xsodnehn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ihgycroz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bljuongu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ikalosts.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bqhrtmru.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2iqoleqin.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tnwbjpzt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fgdbggoj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kspqmjsr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2twzlxddx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2acklbrqt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bbpjgnmw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ifxdimir.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2okwzrylq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cpwhfjji.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mdtuhrov.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hvzgbqwp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2avbkpekc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2memhjzfr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2paqvtueq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zjdkswmm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jumgevhi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2cvalvetq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gxmquhrs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2iyplhxcl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tpoyccdq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gbplrelw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tfgznkzk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2grxtotfl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jnwpluxe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2pvguumxh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ocjjjbfq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zrubhrep.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mwoqaaty.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2nqnblnqc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tiqnmezr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2avlnskpo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2urctetdf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksmmqlji.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2serjsatd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rbmyfdrq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xgwinrvr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ywohxnst.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2boqvprac.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2egiyrkrp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2bafzbtrz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2anbracyg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ixolvste.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rnkohwze.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fibpnzvc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qdrefjji.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2laiagvhi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wkywjqun.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ddrjbvpy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2yfqcnjut.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bljpwcki.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zdpyhmtc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2htpvsfwo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rwuumyzn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mioeverv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2owogkjpb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2epaplegi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gpdlsnww.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ughqefrf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vbjnfwfu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2mxernrhr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ocrclwlh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kpyusowy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2sfwozdzw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rxhrxoac.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwxhnnzc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vqtxrtnr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2spwoaucu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lvpjcovj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2yqdjpiqt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hgixydeh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kseaydub.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vtgybiwx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vdisnrmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igffnrvq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yclbizwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qlfzxfyx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jidjprdt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2simmsird.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bcytaiha.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tzwxwwvx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wwrbowab.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xlvvcclp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lqsurlai.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mkipnswp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pzhddfhd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cmgodnto.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2llloajtt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jijspruy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vzmahzik.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pxoeyuoe.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hdukmebd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2djnbhnbk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xkwzxbhq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uqywnqwx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qnnmiqwp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xaoswgxa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2iarahwwx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2jhdeezkq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cagkzhfq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kamdqnls.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mvdqzoiw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qnuazzxi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cwnyilsg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ytuepxim.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2miylatdk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2gqgqjcgo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xaspfxlw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kwmqfqdr.html


<!-- 参考信息 -->