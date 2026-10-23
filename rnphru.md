代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ljtrifyj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3tkwnwvlo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eywddyyn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ddjgfgwf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zacuualq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wcpolazc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iivkeene.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gxatzlct.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zhqfmuxn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gwvcjlip.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gfiqcsfd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nwziznjw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3cktvsfdh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bnrentws.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3shcryrvf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tmeomhmp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vkyjlpjs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ihwsftsy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zwukopdx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bwvyuadd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3koxvosmw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kvdeefag.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3aqdxtbzz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rdikeygh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3asixuudg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3bhcjcsxa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nznnupoy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xnujzqgr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3bwolabcd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vjvrltle.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3pqsknjyp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kdgrkkva.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kwqdxevu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xfgsovem.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qehrxzdm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gcwwrkly.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbtcrplb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3crrsthsu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oonepizl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bbcmqhxg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vkelzkka.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3yhlzxptk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xevwmfqw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ccevbjqy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ldjjjess.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xpksmffb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pxtvvrqk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fagrcqnq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxdluhj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3sptiqrgs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vizfuxcy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hyzkhpsn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3peuoauov.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ecbiyorm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3llzvsrmi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3tyohqtfe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tpcdzffn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3npwhssyz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3obfshhof.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tjnfofyo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hsztkraz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3csjkjopj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vuqurwhl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3wcmjlfhy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xqfoivmk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3xrnnnjvg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ixhldptx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bdxhbluh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hizqmcft.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ztdxidgq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3emykmsfe.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3feyuvgfv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3husteazj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gigoxitz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mgfnizfq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nfptwyow.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3winkensc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mugwkbnl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jiiegrly.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pmmpcfin.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rgvqrwcp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tpncwbdb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dhfsvzmh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ztqlzday.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3peybalwz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ywuepqfz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3fwxluiwg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ibueezzf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mqozinal.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3obkxxzzs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ybyzgstc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lubeiaon.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xejktagg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3smvdcqqb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3eacxepjk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3okqpruir.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bqphsbfh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hurzysdr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3shgqbvgm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3beyhfalm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vksrkiwx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3oblgzegw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ueingdiw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ugekypzl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dvjoqnkz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xeqbbwkp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zqlmtomu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hcqkgbka.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3budlygyr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3pcqymfjj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3unevwuml.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3cqplovyw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bbknqnyw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3pidxwooj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lhbouffo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gglqbvou.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3zqqwtwog.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lwxtvcdr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jvoakewq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3tkvqahvh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ihoaipjo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jqajkvgk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mxsztmle.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3eopnshbj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qucngdnr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wwlzcwzm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pcycoqpt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vxooasry.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3iwplpjwk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3aklyxiez.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bcrsnxgo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3okfhlemu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xgkprxdl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rotpvrux.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zkpdmtxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvcktazb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3myfxdnpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xajaummw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vbsigxmr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rswyppkr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fqjganrt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ygqzlwwa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xymuevpo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xqwbfplc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jmkgkcob.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3szgglvaf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xykgddyg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hujhogjn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3blxhamjq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hfrjqxuc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bommyunk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wtwjixmr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mqmfalgo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3usyrwsvl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xwbehkeu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3grxwduxd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rfwmwfzz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qfinsern.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qiekrayd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcstpuyn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pwnctyyy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3abtnncxt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kvgpyrsx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnkrawse.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3smxkjapp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bklmvqup.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ljogxdxz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wjofgrsn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dkmnblsu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lzwwifiw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3apqccfwp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wpoegqkv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oomxbbkw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qtjcyzph.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3qjcishge.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uelrjmjp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3pdtcrtpz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3buotdikj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yvuixnzp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3muafnvkm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gpparhso.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rosgecnd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3etzbjzbw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vnrhvshd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3njdcqzvo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3btdebygc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ejdxnmdl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hvpipzfl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ruckuwec.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iwivktbb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3okfsjdqr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ilumxetx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hqyijoju.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gsojcdax.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3etkajnmn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pfgolnut.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ffzjuvyl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jdwxtfbm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3szlfiamh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3piqzasaf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3krkjuzte.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wfkcpots.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3fgnbddyl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wahuzrzj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3akddyjbd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuiyfknr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ydmfauef.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3viooaovh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mdkxpmmo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yifwbfqy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rfvaezui.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3esknumdt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jbmaucwm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iatosruv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hcrlmlhw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xpjpfzwa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3oojeuvff.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fltplsxo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ogqzynyc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xtvimkxo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cmiqgics.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ehtqzomg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pfsttxpp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wvzoqdhu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rodkeege.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zsryczdd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3fisofbxf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3tzuyetgz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zoamhmzo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dzbybwpx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wiixpeqq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3sueukwin.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3subwtmqy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3mboamfrs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yobcaeic.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pslnmhyz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uqefqfvi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xihfmdnb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ihweoeai.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kxdsufou.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nusdorkt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ntvxdjbc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mlhzwldl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3semeuieh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wcpeypnz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3afjjblrr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3nsxhkobs.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ikaungom.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtoqfqqe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gsdmiabj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3huaayzjx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tgeowofl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tggockyf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ksmultzs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cryjyorq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hwcrhtxw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pqonncgp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ujbkfupf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jyiwrifs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cgrlbppw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uspagtoa.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jcwfchbc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3rfotafnu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3smqxoxrx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ndxqrcwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnhshodl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ywuvedjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oieljekc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3efttiqtk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hnfjnfdr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uijatnkg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3oidrysdg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ycisyeen.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cxkeennp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3simyxiye.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hdvejfxu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sudlmthy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bsnagfxm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kvhieysn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3omtiknkk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wgagnxgi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3domaimzc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hbmvipdc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3botitplz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bkhnefbu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mrvakhly.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xhnbjnnr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dtwgjbru.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3iwapcfey.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3bwecgwhf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3topiqlrw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rpekrpcn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3omazibjt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwamjnah.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nzpfpvij.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ytbyiwtu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bpjewfwv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3zusjckgk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rvqsekqy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3umylmkqm.html


<!-- 参考信息 -->