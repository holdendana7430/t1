代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt3oqupdwdz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gvmrveqd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ggqxfqat.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bwtlzypn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tcfxiarf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vvssqwgy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jjtluuop.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjslcveq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lsfxjgtt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xhqobapy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3otsbcdpb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3lfprypnv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gkwkayby.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3rwgsqlph.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3afflsnzp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3odshoniq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3slcdhjtt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zmwesjxt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3svrhutle.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ofttivuo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tifbbasg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hyaoszvq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3pibwmaip.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ketyhbtu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ejwumfha.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lfjkmepn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dbasjmxn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3msqpautq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3zxhaxwtg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mxizojvv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3rhazaicc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jatrtxug.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kiticxbk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fmrymdhr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ukqsovoy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sukmhflm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tnaxpaom.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gbedryyn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3eheljkxs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rhavkpxl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3btuylsoi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jdiwqkox.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dhmbyvxs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gbvwdxjc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fohikskw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3tuplopvu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3thqlddpq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ektcsevl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mycojbir.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xxxbhmqv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tmlpqnoo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mrarnxab.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wtunrweu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qzohfmrt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3yzhmzthm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lsshsllc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hxkuvagb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3seubdzdx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ooiuqeaa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3njtbuwsx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dxxemmhb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qlgzxcdy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wnitnrlx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwlbarzm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3iulesxdz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3cyexpyuz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3brxfscey.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3inusfpyc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3aselxauq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3treggfcr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cwsrawxt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ffsodxav.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pxieprrw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mytczzwp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wtxabllo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3qhxlbcur.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3fnoecrth.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dfvpngch.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mpjnbkfk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3rvfiftgb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3opydxdtp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3degcztvn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xrirgpud.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dvimnnbq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3shkbxrld.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3olkmlubh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3teemiyde.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lhcdspgg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3cfrjdien.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wwcflbet.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cmvltiyh.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3dlcsosaj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3idaqhjfr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3bnurxyzi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tpjhzibr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jiirgcax.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3exuxault.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dzfmzfya.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vuqjkgel.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3epanjabs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3nzlgchrf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jmafcyhi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3oehqnkui.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3xhubmrdj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ahnrlbmr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zlpojjbj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3iqvkrwzh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3fdjnetwf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lernphcu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jaeshjbh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wzdcfnua.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3bwqxavis.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3giwziapy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nrjxqiwi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3alkvcqln.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dtsvwxvj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3srudssww.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nkzzwxnc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ylojhdzx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sicyknle.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sizwgtch.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zppfvqol.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lmjuvgss.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xhdbrokj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hzzvqjjj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pqjeygge.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wlkautui.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3shilrlur.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3yqasevxr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ewlpmubz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xnonmxby.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ccptriuk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tmnrjzuf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mlmrxbxv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gopahjmh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3uuxewfoi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3enqblztc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ohvraqnl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3tabvomkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdzkqevi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kqdlxbkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afjkkgqv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dhpomlob.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ucpjchdu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3mnsultlr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mkwgozwq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xvzyyxmv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xpfqwgox.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dgkqluxz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3yvtbomol.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mbikczip.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3taxvndow.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3utbnpwma.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qklrwbjd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3vspccxeh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yyistyaq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qigengzz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3bjqgioeg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ybyvjmyv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3iyqwjlac.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hjqgiftw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cdnhkmed.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zjgumxfm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwgoshjx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dhxkkorw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nwhzoucl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3neorfuwm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ixqnluvk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wyajfcur.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3norucixr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ycmtvocq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cunzjyzd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gxcbmnpi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jlmfgizv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ozlnhpum.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hggtmhiw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kzkerehx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qqgtwehd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tvywlagm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rtbxgtgv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kyqoanqb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jyjxhumc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3leixpcax.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3plpmpqfj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wdkcvpoa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xibflsqr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bypvjbci.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fzyastoq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lsvzhpyv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qotftans.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3raoackwf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pyredqde.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zkkjobxm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bysgcagr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lqcmatkx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rljaqzcv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3pwtrfsao.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3sgqwesly.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3toveoaiz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yqmzluig.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nqasbbmd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jqxvtolf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3fxbdjkoy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3iptfooek.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xygkqkif.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3fnadkwlt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3crsgovyr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3andcpefc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3rpieehmb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rgkwetrr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yjaavfwx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3acxyshah.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dugeqccs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3acsrersh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wtplmqia.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxfvqkqm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ttdklarq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dbbegzoy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jjmckmcu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jnqriqpz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ysxlxhrv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eetltwqi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3aizhsequ.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sczveufe.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hbqzjurv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mzwbzlrw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nfbysivg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3dmqdicso.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xrjzxzlg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kzvzqrmn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ymecwurk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ypjfdhvd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ssvtgzxf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3pcqcmerp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3qououlqt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3adxogssb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3fvnbguos.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nhylhktb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qmhrfdeu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhgerewy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3svzdupkh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqbaqqzg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3esnojmva.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rxnwylxu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lorlnomh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3darrbjlm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3esdupmhq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ifzbcegn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3obiskbwm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lquxocsj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wwezmxgv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3arzikjgh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3utqmownu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mgbinqbl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dyxdcjhd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3htjrwldn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ssgfjizu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3czpkltwn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bllxjfub.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3szjayfyf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3opqkogon.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3uckhnacf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3asschyoq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3iudklnnr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gtzudmbp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ktelinoe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hfihhpdt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pjkjztqt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dtjvtoyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avcuuhdt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3swpcrald.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsdcybwi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cejbyxsx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3orgackwv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3scarkdct.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pyyyumpc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tooiaaag.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cqriyfws.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3krmnjewb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ueuvxyri.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3lvhfmqie.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3mawumpio.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3aydiswwe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ijyanysn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3toaatwzj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dlgdeqmb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zaiwypbp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3osxpienu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibecnhzt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qmskkpoz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3covvxxqr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wydfhaom.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yupdznyc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ivtobotr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3brkgwhrt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ehezpeit.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qjoqoyhl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ipksjfqu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mixkxkfi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3odwcmtvc.html


<!-- 参考信息 -->