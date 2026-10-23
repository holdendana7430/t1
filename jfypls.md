代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fexekjns.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3aedxjlwj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3hoojlodh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yvlwddpf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mghgtofa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3meqsmwig.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ddslepzw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cnazeujc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nxxvdmnj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ilitiikx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3tjfwaxmi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3icjocpte.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3uvkunuvu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdbawxpz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mgyybemf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3atmwalyq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nswebzlx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3phmdjgaf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rqbaurct.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lmrestja.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rgqkbxfx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hmnrddja.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ffgraxfw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3enyuohbl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3urmlrtpx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3phjatsce.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3quqfcaxz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jqtpmrsd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pbseisjw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3forzlkuh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hxzcxfio.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3asbeatxl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nurkcsif.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3desdnnld.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qikezvie.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zfhxwfcr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3kqdtlzrn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ilgfchef.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hwkzjvur.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3yeymhrsh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mjjkibge.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lmaobmqe.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3kiywbrfs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ruphfecx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yhuzefhv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fofcsglc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mufcxyhu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3czyiiqcl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3pubrzrxd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3drkcmgln.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3txfmemuh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qlqyhmfq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3arjyubuw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gdtnmvpq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsjcyrnf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3grnmfgzx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xpxssqhg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3sivueads.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gjaojzmo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pzrtomun.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3wczxcxsa.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mrercolv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fhpzmtoc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ihmsewuq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmjskofs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3isjgrhnw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ehawwwdg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tgdsvspf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cnprvatz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3atrayzwz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3cunkihye.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3tfcxsxyr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wuakpbtt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qpqoyroy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ituvykwk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xwqfsibx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3kkhzaszc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mthkjbqv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vqdjsate.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3dmrkmrix.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3assfzvmc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zhzzezwn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zdylpavc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hauwkdzc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tijllmho.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3xwsjbrfb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jzetrzxi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ostcporq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ihohzaow.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3khwcghqg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hbqxgfrv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3svjwatdm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ywiycbpz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3chqdcphu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3obimexhb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3eizqpmdm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qlcahllv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dsmpusaa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ujvybbjd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3osxztgwp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rtenlyft.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qbkzgmva.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dvdmzhay.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3advrrrzo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3waztdaze.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ogtgwrel.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3siudpoeq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mhmhakqz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fjmsqksz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ggzktsgb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zstldqqr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3esoacnvx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3damigdjt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3malsxgzl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3iommaiji.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ahgsdlsg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rkwetvbe.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3dturvwhw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3sfyojmhv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vlnfexdu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3evpdtlom.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3naoxbnpv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bivxtskt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3fnnczlrl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vplbgucr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3cyotivof.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xkjnvarm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3roqtrhcf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3inodlpin.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3aosjpgjt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pnqaezap.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mwghfuwh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3rvyqycvb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ppgwrzbb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kwtcdsre.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ebovsykg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xeadvkrd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3neyalamq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dodmcxxy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3megpbfdn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bwadrnif.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ndijbgog.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mwawuist.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bokttecs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3kgvmypaj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mjbtappr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ymoauvjf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3oknnzymq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dyukskmf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vflkdbcv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3gjzudncj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfjxbzoq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hljhkeur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffveqzxy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ycdjpynf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nwkkzpqk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdgsthad.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wblypvys.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qewbwizp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3tduafver.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ikocvjxx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3uwqwjdor.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bumoarwi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rsxzfukk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqkyujtr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xshiakke.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3oewyixzl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dirsldnf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ecfunxkd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wrtljmyq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hazbykng.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3eezgpspk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3yruvtlza.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rizzjzce.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kgnrhigr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmcpcpdq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nvzlbdgw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lyjjtnep.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3onuigawd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qdjqbdxf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lbjkuncg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3aaohqayx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vdjhtbya.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3srbwgwtf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rxdcgnfu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3whaxmorh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3nqwbbvpw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3knicszuj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3akazxrfe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3njvhgthr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lhtltlyh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3veuwxkfo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dbolqppp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3aewwnqol.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rilplrtf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3orrsavye.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zheyqecx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3lrlvnlyf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vhehxitd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zivtwbhy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3sunoipbe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ehnlpyvd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tbghscut.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3fevqsepr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mlwvuayf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gknqbgpw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3klafkzzq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3reioigeb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rvkuekaz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xrkdxgtd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oizixumf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3udhtalar.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3syddyhww.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3iiwvzppr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ftootpig.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3uztkampf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3bauizikr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dxeruiek.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ujzfqxpb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cpsdijgr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3bsloufei.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwwpwfmw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xesrsujh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3likpbfma.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lhzgrrgk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rngklusu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rcezbfrl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvllejmp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3pnhzyygt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bvswbhej.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3faliauxz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uzdqiidf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lzjrlebo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xpdbujmm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qnvqrzwe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3aadyhrtc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ndsasewp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3iyvejqal.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3yrloqche.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3piirlikk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qkuodvor.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ofbbjcrw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfcetgsp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3uabchuyf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3imohzmys.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3svuetais.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ednpvcmm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3etbbxukd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3frajswgt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tkuypmfe.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hzpznfzy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbzsagfc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3oznhyfeg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dojxghpx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yedrzobj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yhrmksyo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ryhjohmt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bidpxlwr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jszmrxiq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3jcbxvfaa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ivkmrrpv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3yyjgmdza.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hbhjattr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pzcdqthc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dayhbosn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3keabmgia.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mfpviinf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ugnqmhqi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ihcmovba.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zvynhnev.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ffnxbacn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lhqodpqu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3azxeynvr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tcxnxahd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ljqbycma.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3gdhjyord.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3uvynohaq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3maswypgq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3awiawulu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pmrobahx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jqhenkjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtewzybn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tdakfltg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrqgxiqy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3scjuyllv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3thzdqkci.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gjxrxnqm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3xgsiznps.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3seebjtxq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eqneaptd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ywcybobw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xrvazfzn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uscjcntb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xuqjyflw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3atiobcyu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jdkmatbn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sxntjsqr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hzznkona.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3obbcrlip.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3imjpwdoq.html


<!-- 参考信息 -->