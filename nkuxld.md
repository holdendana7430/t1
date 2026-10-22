代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2snsaamyd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2muovehcz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gkkzlboy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2waqtjbxu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2lsvrcdds.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yeygcxvz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fnxrhkkd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rbzduyfr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ilqftsjx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2heahwcje.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xsvbglux.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qvmobugt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ugrtggiu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lkixflbh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ofxyoekx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2aunawlix.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2frwqfxel.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2micwkfef.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oysremsi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2azthmqsq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ndvcbnza.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ifrvphwn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zyutcxnt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2yqhgsobu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cbsxmhnk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lqqpazrd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lnhgtxjb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xjhypiup.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jgoaugwy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dnutvgax.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2krjxabgo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rnjhssap.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejsinlvh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2qmvvgwjj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfvfgjsb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ltsdnjgn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wborsnfz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2brkdyntr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xecjdidx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2oougxnum.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nnkbwmwf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zdaarjsl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wsblpyxp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bffacirp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzffxdxb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jryajzwp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2yhdbrmhn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mfajlrko.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ziyxvgrs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jocqvkiq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2zmtdgyvp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ugmohyfr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wwtazhfj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2sirvobuu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gewsnzjw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bakykdnz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fiwlivbd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gdckdmip.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tqlklcig.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mxvkdfiy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mnsducgp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qgtosgbq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2talqjmto.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mxglxrbo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mpnptwtm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gvrcvuea.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zduiifrr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hebviklp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hfhcazru.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hqazblxj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ogfytdhh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qjugkiul.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ckffizox.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jdmhfpvj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nslsqwps.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2exvfhffa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ljksilol.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2okteukgz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2datpikcz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dapuqdfg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2efwkckpf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xlzntugf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kowsfdht.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2brrpnnra.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qqdftapw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2eiudybdd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2woqzytwt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lijycmwr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zogkwfoq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cwwtaigj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2asnxlqxx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jgvqjxqa.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2pbqtpqka.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2woswxttq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2oashulnn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gfqyazvt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2dvkkclbo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2yvmdlbid.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mghpxflh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2cnunxabf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cbdfvrzm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2udpuxftx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2uugulwez.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cnuovtvk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2duelnbkr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ynthttws.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ronrxnyp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2efrogelz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pyrvgtes.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lmwnfkhc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rbqawoqr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tnuhziqy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bajkgbbw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kkrxpwjt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wfvzdllu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2yytpckxw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pckzheei.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2uvwxlmhg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lqfbrpjo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ripbqeah.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2rtnholnr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2afacbsno.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sxjgumex.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2urchfdxm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2hcbjxglr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kisovwok.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2heuhiyiy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2owomoqdf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mbhaxunj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mebyekge.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2yvtjgsjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plnregjy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2njtevout.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsehrjzh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wizzyvpd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2sqwbuzds.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2oaesfjjo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cfrhiyhw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2exadtdrq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ymbymhpe.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ftykwtts.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2alwrcrnz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2cifbyuny.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oxlkjbng.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxhlvvea.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2svqzuboo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zmtvqgjv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2auweequm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2kaisfdzy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jkqrtvey.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jgdfrqtb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wskaumnz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ahthiyuw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rotpfknw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uindoyzf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2llnyriww.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jpnqybtm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2moxunktu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2aklpxpsa.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bwzcczlk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ybbapnfe.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2mxsyqqqz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xsvpkcli.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2tbimtorj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kepnbsse.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qisfiqko.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fsghzxbc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rvqzfkzf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tciwmswj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xcidlqru.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lwlxkzpg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kknarkjp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2yfimqedr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ogzkwksu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ibayhdtt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vijdieht.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xjgktlls.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zvivlrzh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dnisbjul.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2amlqbhxg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2izbczonb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rfwjfqhu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gnlzigwy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tzdyfcfs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dvjexqlw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2uzzrliph.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xtfgeyzo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2pxqqzska.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2khrcewji.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ouqsdjim.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2myuycxrr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ewaowixr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vsrneety.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qpdkgejs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qucixbuw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2buaychut.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xhzqrpxy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rtabvxmb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2kyzdsbbb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lismqiiw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2szwmppde.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jekqzjaj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vbpwounc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2iyvyagrv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gaksapyl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zfgtnyuo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nrcusiwi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tqnmrope.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zralwcbg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ggsnrcoo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2cooobrwi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gbxgvbtq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qpzitobr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qlsskljh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2pbqcbvck.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rdwnfeyh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2owjvonzj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2uydzfdnm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ntalagbm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2epdlnavl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfgvwucn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jytcozbo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2muimnour.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2giimpkkn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jqozilbb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jtrtoyxj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dizkuoyj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2wgqzfiqp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ggiizdkc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xxeglnuv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2mmbmvvsd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnbjsxk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vzlukygn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkwsatso.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mgqrfxtk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fegxmtou.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hmjjoaao.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dwpsnusb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hwttzsya.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2eypjcdbr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zbwxjdaa.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rrborpco.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wsqddeyx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nvurqghx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fndvlfls.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dkmlucjg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rreikawa.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rdsmyure.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2edvbcvkr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ceijmgra.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ruovglzl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xzfqlifi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2taaskuai.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rxloxkht.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dukehsrm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vciuvvyb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wyifuuhm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2imdtnjuh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pipgfqwo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dtzicdjf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eukmmgag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aishgtob.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zncjumfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kersdxfq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fkuzjgio.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iasnvjpc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jrxikmno.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jsehyyvd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xrzkjagy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iaxnwphy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2splowcox.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ihjzgtns.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gvwzupfk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vkzfeswq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bvwbllim.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yqxfwbmo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rbdwdxkf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lajvfkge.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lbrmizqe.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yerwxgdb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ullhchbv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rcqanidy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zsdpjtfn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yutlknaa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ikkencgi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mgcmeqcm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pswdzaqh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tbsafxkt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2obtczkub.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2alngpnac.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vmwfguaj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hikxqbst.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yacjhjgv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2huhsnxma.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bfzsmkiy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xjzoylpg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fclgnhga.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hvkmhfgm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vspyvvth.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mikpsamx.html


<!-- 参考信息 -->