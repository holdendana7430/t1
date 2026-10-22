代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rbblwvld.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2rkhjbxfc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vqkbaphc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uaoqakdq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jqwzmofo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hmlumyjk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2whpxgbtn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yunqfrtd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2camfbfnh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2laxhfdxn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2pqntfsoi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2goiiecqa.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nrtntwkf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lnbhgrcp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zfrghqhj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2prurhrpj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fyjsoizz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2iadvoxgl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ldrmzucj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aqyjwbow.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wyshaetm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2brtkvlmb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sxihhmjk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vjnfamht.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ehifuaqm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qkxbrtvz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tgtjhjbj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rwsunlma.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2guedkdjz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mpgspbhy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bwjvuudx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nkznjxuy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2sktqeybg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qirhvxuo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2awvjbrav.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yrfyxlvp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2onzuynif.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yafiroqi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2laecdxnb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rxucxsmx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbyemvuc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ccrtqvdv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ynuwmrmc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rgtsaxft.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gdxzyxcf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hphevixa.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2afmutuvp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vngviwoh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ixgunalr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cqiqtzer.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2bwcbhsqg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zpvlrbqy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snaiuzxi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2baabyhgv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uipkfvkt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2heqjcenl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2hpwdcqnz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qgztkrca.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mkwimsrc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bvzkxqtf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2azkgckzf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2duhsymls.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xqzlhmxl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sbqoqpyl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mnabkexw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2wtbaiqzf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2cawkffpl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2isupwvpa.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rnmujtok.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wbmqvnal.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tcjgghul.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rfqwjeyv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cuamtpft.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hfpvypaq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2iyddhhhl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hurvnfbc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2spbxvgyr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2wkobladn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2acastmqt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kxwvmnkt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gnffwrra.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2yaffywkd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qqbnbkly.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2utzvdwhj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tjjwiqdt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xohoaces.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wtkqkgiv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rtrkxiki.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qksredsc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nwvsulii.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fyqyjfyt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ybpxvwld.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2yocupnak.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xkpuknjq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jjlekqqr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fvidoplk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2txuvymxa.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2olxaidfs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dzmkxbni.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xhlwrqld.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2buzydwpc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ubqizmqw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hcqgtwgy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hvfvgtox.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2exnroika.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xjbdtluk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hcymsaal.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dlpvegzp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2iqdafqcz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kpgqfpxz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ljppxvpn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dxycfexb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2slwtacwi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cybeofon.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jlskqjax.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2enxmxwak.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vznddvwo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2kgfszyuo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hqjwzfyz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wijxybwc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qicbdfcw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jhmpejrb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2nhoktktj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lnyglphm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mmufggie.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2vsvoquei.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zsvenmfi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lfjxhsxd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nntqpyoh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tvjrionf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2praatlgx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lruudfap.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2uczeqpke.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ecwflbhj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2viaovkvz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2kiwgugws.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xqxsuyqz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2untmethi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2salqqows.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xvsbzvpt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2szpaepri.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hgkaeati.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xcfnmttd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sjitftqv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fdjiccpd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2efzhbhlr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwdlgzdo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xdnlnztf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2oexamzxe.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xxhyicgm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xqhelehc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlxsjopw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ozfythek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyrgntxs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bermftre.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2msalzpsi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmyngfdx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dunlhdcs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zlvhqdkj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2asdbdlja.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jalcgxsj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yeorpeja.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mdhgrlbb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rdkncoxu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lmrvnrss.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jeyrbbhh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ymwcmnks.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fasnuwwm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fmwctsfi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2axhydrvq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2zxabagba.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wfovhdbf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pfqpayox.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vmbkwgas.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xrxnldfh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gizxsmxd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rrdqxkyx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zalvbfms.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2obikyiie.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxufinqb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hhrnmpod.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rcznnhsw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2oiojvodd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2unowicua.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2exetdpjt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2thwysrbq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cuhbbcin.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nzeuywqs.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qrkvfpgc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dauzmsav.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2npkyensd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oqhnwzex.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2poxjkujt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mofvgjhc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ftdbvxht.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jsbslscq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mevskqsd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lkkwzubi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2eferfhhf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2eyifumde.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2iwnluzbj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2txkqdktq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ykpilrhn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2cisfeijr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2optqnboj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hqzdazar.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2noktixci.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cuncxjaz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hfycjvcp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2knzxhxvd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mzryhhsc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ttmhxvux.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2unzquros.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmevvqzb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vyypyygc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nlnenhcz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qzbmbmwt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eicuuabb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ndmqlzed.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xxunsbxp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2glzhqvbx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyiwvinw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2paxpskxz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kuzkzmag.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2uexsdkjs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2demnjxuk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2roalyvgg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2trqmxitf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mivuugqj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2stwsttdn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wihsluon.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uersbzrr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ofqcbymw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2idgahtqm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ycldrubx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ylbkxncp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jwyejmmz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xlongkze.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2cjabgcmv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2rbwecita.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hqkjsnlx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hqjeygjp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ocfncoum.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jlgypivk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2aqzbojch.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xcdhnodb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xcgmkaav.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2irnogunt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fkywpybk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ncsqbmdw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2bdtphvqs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2onkrowoo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mkhrmxro.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2emjfmthu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sfczerww.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mapidtvs.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sxnsvavb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2silcimil.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2eyfoyjah.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rzacvbpi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dlikhhrb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2puktodpc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2diwoeqpa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jghwqulz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2whyjhvvp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rmxeouxp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mssvadss.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wafrmnuv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2gcdahmsk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2mwtqpsrf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ddfytwnf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ltdzdcwr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qnycgsvu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2bhlobhdu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gyxlqrfb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gykzimuw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ylhagljc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kyfabyno.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vhmztjeo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uwfdhfwe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2enwevbcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkgefjzn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ywzovsoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffjbdehc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2svhawcur.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iokayczv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xxopwcyx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xhpfrttn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kxigaagq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zqmufkvg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nofcbhft.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ayobfweg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ldraowau.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2zqepzrzy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cbcfndfw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xelmfkyd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lovxkduz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2utxnhict.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2chirjotf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2roipxvrd.html


<!-- 参考信息 -->