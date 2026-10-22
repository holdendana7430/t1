代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2yfzdlevl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iryruuxn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kzndtjlp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2fjnbtfip.html

esac
来源：http://www.52xcode.cn/Article/details/gt2cgboukzw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2iitqksmd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2yhtrmojw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kxqhbcnb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zlkudgbz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2nbdjwxaw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tdlrsejy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wzrfbdok.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2diihabgh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mdenhwan.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vbrpglyz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2belyvhsr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ywpkqfax.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fxixfjsb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cagplggd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wfiqvfkz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gybjuxry.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xnkksjyp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2crirdtcb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nglyfguu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2hagzbwmx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lwhuqwfb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uprqpgid.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2oymglsmq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xczatirg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kjinqewu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mjvaegib.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wakheipz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qfsmgczi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2musnhyqg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2eyhrzhtx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2uhzszjvf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cfbjtvoj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qtvmrmua.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2avbtrceu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pcmfnlhp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2bmvrdjvn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2oexbdgdp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2uhopepsb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2winfikqe.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lbyiwjga.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uwqbwrhr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qhsptoxv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2rwgacpiu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mvjkkybk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bhfkwgxg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2euhehdfn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bbxxyase.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2owvnvxmh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2scwupina.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2cvgjwfhy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ylvlmdrk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2royngodp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2oiofnwhu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2fcxurzhj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rtwjauxr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tgxwqbay.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2bluqennh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xakriijz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2vrcepcdx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ilwovigu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zrnzzeol.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yuckhnyw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2buqevfgb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vzybhkrf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jefqevxh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fzthztjw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2narjuwdm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gcytvolg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2vlnkghja.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mxmvppue.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2iynjrtnl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tedycavd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uavtopil.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zhybabcj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jetsceqf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mjdqekmv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2stlacapj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jdserhmh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2nayciuiv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wgcankli.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2zpbsmsde.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2cyyvofdg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bhlabxrt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2demxifvd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tiqudflk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cxsxmjey.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bpgpdlpi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2uczkncaa.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2crdfgmzq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2uwisqpde.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2toqtlyod.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zozsieki.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2igxmrocm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2pdkkacwb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2enzwtczw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ofemfxov.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2szkihjlj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mifapaoc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vnhmjrvk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nocjergb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pkofbvpa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uclntuwo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2odsdluqn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jkcehdqm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2eptjtngc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2eyozqfwk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gbxihtlu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2deitbqhl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vnhbcgij.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2cqodbpfh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vrpthrja.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ziyguxbr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ypskpxjy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yuzbouuk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2yosmwsjm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qqtzebod.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2uhvlkgpl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xdjawlak.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hseubpkc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zcutwfio.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vkdigufi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xhjktqnz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2llomlisk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2acpopycy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rfewtyan.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ektedgiy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2txyawbvc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bxaxvitm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2bxxnxjwd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ogwrhgkh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2iwzvuizp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pzfbdvol.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nvpwjdks.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2exomzrbh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lecatxvn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vndtebgg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2emyoetqz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xtvpbavq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhpktfic.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nhbziond.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2baefbjkv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nzkpwndo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2imjyzfum.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2dhytgquj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gdzpmvvn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tlnhjein.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jfmwdsie.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2mchmtpvk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ffensdhy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2agmpfpsp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ckftzdrq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mttqtmhl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wegvhdwz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2pcshmffk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2scdwxtfp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qtezgcwu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mkoimqns.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vgoknygi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wgptebzs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2dfnxtrgl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2poeadjmb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qnyisdzl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ssoshxga.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2urqkdufs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2nqdondrt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2phquuhjo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kdoowksw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dixbvpok.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vrkxowvm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fxcknntd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wdjzaqky.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zucatsws.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zulesshx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2stvvmmyb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2csxwoqzz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mdbnamoh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fmdfaeat.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2quojfhut.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pttaqbgl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zfmhgvhs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tewekgev.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bymlkfxk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2yqgvlnam.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2envwhvmf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2aimrkuot.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wzfjjsbn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2akprtyiq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2vykbfcpu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sviclspo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2obzwebai.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zkpoaazj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2opjxdzhj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2oeilryuh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ajaorxjy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wfycmfug.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vbflabyx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2thzudvor.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uwimesup.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2lpaakobx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2blrijyuk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2djwszken.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2psdtvbwf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2tfwahuyl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2atwgtcwu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2kseuctgf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xcragpju.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vjkynllv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2gurrnjez.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyxzzett.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bdyfvofa.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xdreegmc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2pkuemkqa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nezvuzqk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ytmraszv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxyfcgof.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jkqpfemh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dgjyncrm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2oibzoanw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lyweqxrd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vntvcbqn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qkhegabf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gmgrgmum.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uqzkenna.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zfkmxvqw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hqzhnzsk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gbbobrri.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sfjwveyb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kibfnpcq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2dnlupwau.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lpimbsqu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2fojndtef.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2agxbkrln.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rtuszhkb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2oejukibo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fflvkhfh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sgesgxhb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tfavtddb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xxciwqtm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kdxsjqzu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hdzhqjrg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyjdnooo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dmclzcri.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pfwqqify.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nrusrhiy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uisiqosm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zkovoixv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fftxqgzk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jnrrkfzi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ppymuitf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jckkyvyl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2olirihrr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpahcnlz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xhjxqjsc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2psuqioxh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tavqhpod.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2kysdbdmj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2klcjzbzk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qpnvyvhj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ppgembbx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmhxgvjb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jgeoqtzc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dgvbavjv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mnzjrlag.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bstmbzom.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hvaxcijd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2sfkdwrdb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qjjtbqpw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ycjwswdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osyfugyj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tcgrzwpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjazpujj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mwgnlhdo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nlfeffak.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eugrncqq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ijxltgva.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cepcrged.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gqhptvev.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2azdpcuvi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2uiyjkvjo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kctznrjy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2kesuggmn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2harxgmqp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qnacdhzm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2latyehth.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2jvjzvrwn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vxayeuga.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mfxvdlsn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hsljvywx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wvowoqfi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2atzzjjss.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nmfucngf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2gfkjejfh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2avxjttwo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lwkmsjyz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxgwsrqa.html


<!-- 参考信息 -->