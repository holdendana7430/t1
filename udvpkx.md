代发 wailian999

esac
来源：http://www.ydjk.org.cn/Article/details/gt3slaixapb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqykbqob.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rezjpomu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qugadgqb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3swynkjcr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3mcghqrzm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zhocqvfj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsteiaqz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xajqiazs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nraqjetu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ponfqxwc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3oqtfdmgn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zldkxiyn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3djeiksdb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ofqmqavh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bgsblcjs.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vyltcidk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ykkqpzzf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mambdpjk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3afpalrnr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3npxdfcyf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zlhurbwm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qeeaporj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3palxtbwm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bwrtfmjh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gwyzhtxm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3leufzqbh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fzdyowlg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ssuecpwu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ivlrvisp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3pnpxlcpf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tlqrlzmd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jxqrykup.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3cabzjinf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xhnmlqzq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wyxsnqho.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3plddmvgb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gjrozbjc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rpdbgsfq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hejzabbf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeammvhm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3millzojc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tmmxkivu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qtgqbofo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ydjqhwow.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3juizeity.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hzuohchl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rxwwdulp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3lghsnymv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fdydfqbd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ijkaylrc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3sbqbpqtl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zraqyhfy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qiwbcvsb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3cwugpbhe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ntaevnoj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sgxnpqhn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cqavczpl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ijpvcadg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3sbtfozsl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zazmcqwe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3sdaafuqm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fxgtdznl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ogbmdftz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wukfulkg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jsgzvjot.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jydwazgp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3dssyiawk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mrguvxsy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ipwgpapu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hvgxjcyp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3kzvboxbk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3znktxazy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ynzqqfyr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3klvhnnsm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nytkqrkf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3xdhrvzhf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3rnjkwaja.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vqileamn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xgqaphnv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3tcoxtgin.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hgsrxkrh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ttocurxo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3esqaduqj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3aetqxbgi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gzavruer.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pcrbwhdr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3rvcbekjt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zozwdnos.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3krvmadwg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vlwhpykn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hjgrysvz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3imirbskd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qtphdhei.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3szebetwk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3shpoxbfd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qnfvbjac.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lxuuaszv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3whnzkyuo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xfgwzzyb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3pnevoeyw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3adjorjcf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hfkfpzzm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3jixccgjc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ohlpzire.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3uiaqggja.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bkvlfdpw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fyhmaszs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kwnwojgm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rtumgajv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sykhnvri.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qgncwqym.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3nxeurqbg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3epixadeq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdosoizy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xsxcyylm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ygjkgfgz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ifhurzln.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hbfhzxjd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lityfdqg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3esarnfkv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hqnberhe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xtulcahh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3exwezxnn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3joaofyzr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3fqmgqcjb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fxyhpwab.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zotbppwa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gwejngqj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gboxhfsz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yultkmvy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3srqbogcl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vtfxwwrz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3loavixtg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3gtmbbvmo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3idkzsjgr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kurrjvod.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3akpkmlxx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xqnllukw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsthojxv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hjhtnadt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zeftjryd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ktogjbkg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3amtxhmkf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwmxtfch.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3solzvstc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3uhdarjsc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rwtvongv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lwbpuwra.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dxztbbcd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3thtgqbgi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gohqfwpa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kkakbziw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nqobtnir.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pkwhtsex.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3gxuimpje.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3pdftuxdx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wytmqlee.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3crfkywms.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yihmbzft.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3uvjjpcza.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yvnqlica.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3bqncmyvw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fmgiftjw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hunxenjb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wzueshye.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pwyeefwv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3izugytgb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yxeonnaw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ugbudmnu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lsowqgja.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bnsjwnmr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gpbqlpeq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lelsgbnt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jegpdiwv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dvitlhug.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xvkdqkdp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kptjnngv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3iginwpdf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3piiqqtir.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3pyqmnnaq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jogejhjw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3agdtgrgs.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ahpmzghq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qplzancw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wbiiokqb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3psapizzh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3iquanbwo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3prtipbko.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wjsjlmpq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qkbfkqwj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ipjrtkeb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tuyczemh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gtkkajqt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kshkrteh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3nzurkiyx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gvzwfkxq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nlmtuozv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zelpaeyv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3uyxnvrwo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cwoiyrdg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bklocicz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yjdpcloz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hdyhuamq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3scfmahst.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rkfuzpbh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jpwipzpw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qzdvyshx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3oxiupcem.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pcltpzmv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dnwppwfr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mmakgots.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3goxyvnde.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bphxbfns.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3pitqbgsl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxiwlelo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tekxaaac.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ntzyapvv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xgnowjdg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pqtnwsny.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lyrcgphn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dngnaqdf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mgefsbga.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vpulavji.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3pvennchj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3irikdbwo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uuojxmdq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bhmzjfso.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qncwfgnx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qxfocxmm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwmmdeav.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3voragshs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3aaktdgzk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3twupwrbd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hyslqjmc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zpqsmdnn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fhuwrgil.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ahezeixo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3dahotzan.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zcdwmuyp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jmpbvttj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qazririg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nuljorxd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yiczfylt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kswgqfmr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwceewtj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fnpabyrp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vweafxer.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wzdlhncx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3slxnurjx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bhtovmqr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yiqzqyeg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbecgcyv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zkihaobx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3nebzbpeb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uouinmun.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3gtqulksy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3siewfbnw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3cqmdtwta.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uwfscirt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttpfntoy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fukaelai.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3brajzdde.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wnvybynk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhnmzcyw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3esteblgw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3azbovfrf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3eiaixgoj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ntgnvccc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zilkfsso.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3azxpvhdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqeasuyw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uopkibbu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eqrgapfh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jnviyuxy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zyqtcpnm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3uzgokiia.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zaaycief.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3svckvpll.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yqlgdjfd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3mzagmrsl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3okucblnz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3szairnhk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvzbakgq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ngskmnrm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3rbxvlxyy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3oerliivx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jmcrltjy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fznsrfkt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gnnnrlgx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3scuprfcy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3thxqtuxk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bbvjrfis.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3suassoje.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ewrsmtoq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3inplmyky.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fufgohra.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3udngclji.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ckjovpnj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tpdscatv.html


<!-- 参考信息 -->