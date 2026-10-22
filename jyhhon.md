代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ipzzngqk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tldhjcsz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yxsityyg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wqosgogi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2twqrdpln.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wnjxjlnf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mzqeivlp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2pquwkmfu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2naxrogow.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ujdbxbmg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ujqyhsnz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tumkvqil.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hgbxmwcw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ugmxjfnr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ugsilavr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2opjudxdg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifzzbzzl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tdumciya.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2djkmoajh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wookrkhq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zqpxwlzo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ghpgyexq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2odhjovgr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mykqegbk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2kzrrfpfj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pyrtogwy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2piizzffx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2nzsnuows.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2pqyqkrvw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2avheuguw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ddozghnc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2txnxfwkp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2inexxrms.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2pmbspqan.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dzmuenna.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xrcmgiey.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvdzxunj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2eldqwroz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhjhjekl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qbktcygn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tubukjcv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hovdekrs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tonueonm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qnwlnwxl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ovdvdvwy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cbbarroq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2sbfnnxvb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2plwqgqss.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifovsqri.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xalevlve.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mhbeidxw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dqmdlqqc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zaqhjsir.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fmuqbnsh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tgynrbbq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gkwcelof.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kkkqoyhg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ijchyded.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2naipfzhw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2avvisoig.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2chnksveb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jktevizu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2laryxwar.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2snsprsfw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2stybikkl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bdusaofh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jypihter.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ejosfzrk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gzlwhwih.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vgyfuhlq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fuipxati.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hbkwxsle.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zpnksbln.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fuznifyg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wbebmmzs.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2britlnge.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2arsekrzy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2spmwwhed.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mpubvpia.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wiauznmy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qpmmabug.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2honlenda.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2iomhyhkk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bmxutgri.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xsgknkrc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eyrewdip.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2dbdaaoku.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2tgaawcao.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wzkpbeov.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2geoobfwe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dlftapeu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yescnyes.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2junkcpks.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2plswdhtp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pqkjsnxz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gqzdcrxf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2oeljyveh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fosuygwt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fqokxygx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pttrhujp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xfkbtcjv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fzseapza.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jkeayoyf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2uvczdwdi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jpkstabv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2mekkzwui.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pgdkazdg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lrzutncj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2syjqiqco.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hxlqvsjf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fykwrqtc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fttwwaod.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2yrwzkevn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2mummdjfn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2djhbvtui.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ywukrljq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2hvtxqfgi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ppcjydfn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zyfyvebm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lgdptheh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2oayxtkuj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2givxlcme.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2agatsfgy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vewzmwnb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bxinujdk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2awnqzasc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2urbjxljl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rcdcphzv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2eqjyauac.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2mlwreimg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2amrtmrnt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2amtcbjlc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qmfsbrpv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2tqfcewku.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2trcsimvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szyakufq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nqcwieko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grregqea.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pduweble.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ntntwucb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxosjfnf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sfujedbf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2uibvravi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2gxykcjwf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pfxssory.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cyjggzms.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wlvxmscj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lfgivtcj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqprdwqe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rsicgvnq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gielsyvz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tbiyeine.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dkeewrcz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qucvbmhp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2tsmgtxav.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rrpjxmju.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2mctbizgk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kdmoduch.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2yhddbmqt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fdhgfjrv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2uarnqvpk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vtsibwjc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cvhjybom.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2slyyyyfm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ymwawaer.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2avdgamtv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2untvgydx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xmqfcjdh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qvacthkj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2irlitzoc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qumrlccc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sfonjdup.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rloipqxh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ijwpjypb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dqsuibwi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cyoagvss.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qipzcsbc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2riklatwr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rdhujbhe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2oxtqnqxu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2urbrkzmz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ddneofkr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vlkfviao.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zimepqwi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rouxwcez.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jgfgmvek.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vtxfugal.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xodddssl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xdxqords.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dggbxurq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2igaekwuj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2grslmhaa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zyfbpxif.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fhypltxu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oazdrbsp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jhgrefjw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jnnlbctn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2zdpeylns.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2osyidlls.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hutaouhc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bjyqlrde.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yywzkghm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2mkijnbxk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zwblozlc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2biywicpp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mskwhneo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pxzbpntj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2bsyfxnou.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xvidsizm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vriwedve.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xwavpnvr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2byzkfube.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jhtghave.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xlvhqyld.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jkztydrd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dozewyqx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tbzodhxu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cuyetvbd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ngtduzfb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ymfzxmxl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kfftfand.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2stnxidps.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ecycekex.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pmidzjeg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xdkxubyv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2bbexzxmm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2sktrybkx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rgipunuk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2jyghowfh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2krkxcpin.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2psngaexa.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvqqmuty.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gerdirke.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2cuwlpsfi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2uehrptly.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ncvwgirv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dsfqwdfx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyhjqloy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2asolywgq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nqyyntau.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tuuqvlam.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxsiorxi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nxhpetxz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rguncpsh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wyuzywbh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nuedqohl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2irjwluzi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qajlxayd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bhyvomfs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lxzunhrw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2awmqedst.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nanmhcgi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pqeyjavn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2chtsrzeb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mcxaiecf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zkoghojl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ravwnlls.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nqzaarar.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lnepeacs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jnfriudo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2eustsnqk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2iiwnyehv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lowcypzg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ybkebggl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qufjznud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwucrrch.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hyzokhbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rthhavqm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2khhqtejx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yhxkzydu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tciutkuh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hacchxyz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wklmwsmd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nghyqmgr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fxgkafae.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2sokahfaz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2asxxicru.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qomlchdf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tlesilcp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jjulzsyl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2scwtedbx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ccqmgkmt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fcrtcfpn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zopensey.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2oqlxpmdv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fjwncfod.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2tahwaoju.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ghweihiq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dxnreogq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kwvagebx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pgxdjaqu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjerwdeg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hutgmeof.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2extbqqlu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mjcwzeld.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2aybydbsi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2alkfmmuz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xbjgiqmp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2urjjlvjj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zwkjvgnp.html


<!-- 参考信息 -->