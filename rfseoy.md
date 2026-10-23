代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3iqhvdtvs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tfjpiluw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hzwnhnqj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3opcfwltk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3yxlwovon.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ipzkdkus.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fkfmhfgi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xueqwhwm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fqwcfflk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yycishnw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3hhoowshu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zhocjmad.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3floubdue.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jqwcvvsu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dgkrnefh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3affxship.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kysggxyh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dqpakzrj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fyfshgsx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ugmienyn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ftsufqmb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3juynsbnt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rhvrvvvo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3heoumiqo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jhrcvehg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pimuxuam.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mxsyiubd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ynbdkqut.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3svbwwxxi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kmtzzajt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ctsgardb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xqktqjhs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ncojufyt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ppsohsqd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mlbqduey.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kwqidsvh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcgobykz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hvbwaeal.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fbagjuza.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qabsqihs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3smhspbww.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nvwdvwtk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qdmeknxc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hqjqvnwf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3lcqlrhak.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dpbqadsb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3trkhqien.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zwfpuunr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpugsbue.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fxkczwil.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ywqafbsu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3kjtwssph.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kbmnwkti.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mzenvkag.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rmwiawya.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3otoexknj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3biasclrr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3eyxrrimw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3goudetih.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aeyxvnjn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3acuouwes.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3msziltpk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qnrozkyb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3uxviyhtj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3fqhrtxlm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ziqzjfun.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3pcvymxwl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3oxyvtmbx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ikbcgbnh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qibmjujh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rwbfreka.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fnrbyiyf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3amhoubnc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kvehcgmp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3njxroqbp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kvmhkcux.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3xbxyrahn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mfzcuyem.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3novlvnfj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nhfratge.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fdfvosnj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rsuhxxii.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mqytvqvc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3afbadmte.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fwbgmgme.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3mlctveln.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qtjjatoa.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kcickdkz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pbgflyro.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3evybbjvl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3laoxgcnk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3eewuvphw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3lyafmuyn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iirlcwwv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ffvblozr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mmgjtlxi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gzkylbfq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcucizea.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xulaztal.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3gllsmimc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3icejhxau.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3omcgxdkw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gzvhfhpu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jemjlrca.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3cqeurkbe.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mnstpyfy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kwwbhdgw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3pwupcxyg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hcstatac.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3awtdtbum.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3whqwyydb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hjzhapjs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zwyuuvrl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3lquapihf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qyaxmqtv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bgbkgduh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dyujzrou.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3jtdqjvhp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bdmaewfy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ntrogjyk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dytiyokr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tphelwgr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3glrbfdfg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lwmkdmpo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dljgrlwu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3plryyaid.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3sgywroor.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bvecxwkr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3tdmhjkua.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vwcexokn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3djaklzgo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3acfzuvug.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3juywfcqw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gytdsldm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qugbbmyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vseuortj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kthwpooj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eptoarta.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mfgwkoku.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3currvmfc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lbrpzcwf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hgbbziak.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3yskiihaq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3whsabltn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rkzauiuq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mfbtvqga.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xaecvjfp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hnvpcydi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3aufrgknv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tzrhfisq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jmreujqc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3udtuuzov.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ycogdgdn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jlgepwsr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3luwbgjhi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3szaronlp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3znfrneig.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rpetjxfm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3whejngpd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3whgsvqpi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3asscflcj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bplatgud.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ojowqyjv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vxipwssn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3oxciaxtx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3spdorzfo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jlpmzxig.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3avsixubs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gutiesvk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vaayqjre.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jylbbnmu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nladfgsy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sboikyjn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vyjqfxyj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3elwsavlu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zjebfhep.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zcdbzewq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wybcluih.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hwcriocm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wrpxirve.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wbocwhkh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vfyxsmzk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3fqbmiutm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ncohvsag.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jjebwtap.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jmvqvmss.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ifbsance.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3tklwczdd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ikqzenza.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mhsiumzq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3iiwdkypq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yqqpcqfb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gdfveyrk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3siystgkw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3luxznwpx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vgyyhfuh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qnlcfqld.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3stndpzwv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mgxfqzcf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tpitdgyr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nlyhvyjn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sjufnvel.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3woiegdwh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mgdsyzdb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3atqhmhnr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gorixzoc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3etcuxstl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lgcbhdzb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xmmwptca.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ejxywign.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rmmgxpgk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3raaxgjex.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3dyayutcq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hrwhxwrl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hpkiehvm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vpccapdi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ronctbxf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ypoznvwi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pungvwrw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mfynszcy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qhadkkqx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wmybqszd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3suxqzdhf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mvdxscbd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3yvefatub.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3opvlivxe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgxixguo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wqtmsdys.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hrlfmwjr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xsxatees.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ydjonyce.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ahdpdccv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gtaekinc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qdagqopv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ewholsos.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3evjnxlta.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lneylqwd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrcbfkws.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pawyfwnj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lillqwfc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3iwlmjhsx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3lbmqsahk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tvldekca.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bakmwwdy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qckmwwdd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rnayznze.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hrudfgxj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3baomthuv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwodhffe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vziqcrtv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3weegfrgz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kykvfmnj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3raubzfrv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qpktpmsf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bwgnxvrt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3pkrzdtig.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uasatpjv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3djrzeaul.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xhpwtzzn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yuyvulln.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3agrtubwh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jrcbxfqv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3crivhzwj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xsoczrzl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3etjmzrnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtodohbb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3puestiax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3legkyxqx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gpfdshlg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pybfrixp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3panzdrai.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ucglwudw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zegxpzmn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vqpnnjyf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3alyftaft.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3sierbuca.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nvgxurqt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yzqnpjms.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rwmrmwgo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hnovslyt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kwdqmnmn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3azepplas.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3luvnmpxs.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rkpqimpy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yujsxrjr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kwtsuehe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zirkqwkq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mfrgglnt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jmlxfpwk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gajlyqnc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jxaukjvd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vxhvrjha.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jydonrcn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eyewnnnz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3svzezmye.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cgvaodft.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3uktosdaq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ohltwuad.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3batuyaxh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qsyjnjah.html


<!-- 参考信息 -->