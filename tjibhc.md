代发 wailian999

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wnyovecf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fsnadrwf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dpzldvzo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jhwzleod.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3itsuldsi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3taqtuijt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cyfqairi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aqsfecjp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vlympfxz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xumjyrjx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ocfbmrlb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xgvvttap.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wypjuotz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qjonhhaw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fdaydbsi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pcrwxpki.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3cuajxlzl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xidmcnmx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3joxfprit.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pbxapscv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlrccogu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3btffmxzf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtzqwgjy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3awtdgtmf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qtirdrdx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3snxscpde.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfguijjc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3etdlnjpj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3rtbskdxx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pwqbcprj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lftjespd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tpffgbjl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nvusysks.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3oczbucfc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ghaorxiq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qbtcxgcj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rmnrxroy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3onsicmqv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rsxjidbb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3tgxcbsyi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rbwvtibe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gmrrjtlr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsqjxogp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fpclkcsc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3inxufqyu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3lkejelau.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wpilrmtv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3awrcvmya.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ivocacij.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qguypasr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vgvyjyvu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jiyiprmm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nccapkxt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kfulatsi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mnibdvtw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cqfuxxem.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qjpexppk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wsmueoey.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uzxxorwf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pjlwnewg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ipbuwbhv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3stfpdwko.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jaobchzt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3brvaahtw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3rkstfmlj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3sdaoeilw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fnrlgqie.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hivgaenq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lpunkvle.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3koyvpkws.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cudnvaty.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gwableok.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3plbvkvkr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zypofzdg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uurwmmnk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3cykgzuri.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qjlwttmy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3vcwhrjvw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gcwpuobn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3crhozudi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bcciafsx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3beibcysl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3syhimahk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3gihknzve.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mzyonrqn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqqfomqv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qpnuvsri.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3cuyhrgrl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3yzmaagbm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3scjqylxw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3czxxlwbr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3usufelwt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3odyocnwy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3thmomlbj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vkiydesn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fqdkocnx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qkpbatgr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zbhrjkug.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xnvazpjy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hecmylys.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3hkxrldko.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmsikess.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3pbimmdef.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qqxxwvzv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3egehxsyt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qlpumlna.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3rgpmphjd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3whekiyrd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hgiehcrs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nlofbmab.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gkjkwjgv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lbsxsumx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3sanlovzj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bgobeybi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3voorzlts.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gouyqsuw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3suifvfpw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3fhapcisa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3xoqaseav.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mwosbudf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3zwkzvqdy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cgukccik.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ybtvdjgy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ifprblfe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3eexaqufx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3gxmshefe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3maowojzm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3deckbonf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3apossknu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3uabfackq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nikppxoq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ppbmxywk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3esamfcvz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fpsohaht.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ohprxvpu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gaezjnbm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3khevbkvx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bskhrrhp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3gxrqnxrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhdfvkaj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gromjyas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wknuyyex.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jzqjyfec.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jvphgbtl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3txzblozh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3exaqykqs.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wbdtnbrm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3aieudkky.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3qnvhwnrc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3flwmjesy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rcaotpsl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nprctxnf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3agupqfnd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qokbaidy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lqpqfrhh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wcnslopu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3srksvjaj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nwnpjzvz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fmpyhnij.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jsamfqhk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jbxhchof.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3togkqbcq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rxyzayvt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oncxyvxq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hfesbkhb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lnqinftk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3updregll.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hdlolefu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nqvawazp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cfjnsbqi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3xsvdkyao.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3uzhrthnf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3lobazavx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3coblhscn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xpokmuov.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3umdwnipg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ivedbxyy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bwttilgp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ogmrqimd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3oenowxcd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3uxoxaasw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3intgtojr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ccjdbfsw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3uyvtwcxj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zmvozipd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rjmkmwxy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rgeondhp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xtfdztjg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3szhwucez.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3htmeowow.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3klbjvnok.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3msvzfwlm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tlawagpx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iofjeazp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3sgfefute.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fodtzeqb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rwzmciia.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3rzmzzojd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bqqsuchz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3frlflxfi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wkrfxdnt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3azatyfym.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3iseaydmm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bptzotkv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3iotqbbuh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nhuygcfd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pssngxlv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qbryusrs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ljxgcqdc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3uobxxopg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3yfzdntmv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3sqkujddn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dnxrfkbp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xtzveebp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3yojdagtn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bupwfgbn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yhpjdcwb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gtfjtlwd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3softlwqx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nvnjruao.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sgzfhrhq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bqpqgjgm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ztbokoia.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jpulmsqd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3nugnhzux.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3csclqwxl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nogdjcap.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ahccjsyb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ofmkmywg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3adqcbrbw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgvpsprp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cjkbsuvs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jjccdjhp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3unnxhffp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3pjthxobs.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsylkkkg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lqefmlxs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3swurwbrg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3bajtbcwg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqnnwfsa.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yrnnjqrk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovxgnvyz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ewwvpnmj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wzbdpyuw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yskemjnh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xxgudqhg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gvcqhvrh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mixalrdv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3myjjalfu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xtpnfkco.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ubufyqsg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xrtutzym.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3nikjmepa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wtyvfqgx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hysqyirq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vurejawm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jnyaosby.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yukayoea.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oqxuyppx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3wolpknql.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dtywkykq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3sthrodif.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oqfrfmqo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mqlrawqc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ylidnase.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wdwjspcn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3edoxadbi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jsuyknrz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hekvurmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyapchau.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kmdlyqqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3karhbllv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3znvdameb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3alnbqfat.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mufwoonn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ntnkerxk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3dfioiuoi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vfpyniyg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3tohdmbir.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3obbhzltz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3herrccfm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pvhidipc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sblotpct.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sebhqigx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ebywwhgj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3etyqmpuy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kelwmmbd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dbltxkut.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgzdzwwx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vhgkakzi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3enifuraq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3gxzdjcns.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yqkogqsd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3iofvmdvq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xiyoxeup.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lfegpzmf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3akitwjyf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wsvpylwo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3aocobnra.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tsqwlnuk.html


<!-- 参考信息 -->