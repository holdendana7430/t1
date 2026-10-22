代发 wailian999

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mcugadyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqtgmhuv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2uqlljnup.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2nkoxfpqg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zmdcitja.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mamonmbo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2uktlllkh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ibtkhitr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2uhtijbxz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2apizhopt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ifbnjmvt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2myjbgobd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2kxbrqova.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bltsgtqj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixvgwurz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ayeigfhp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yfblnlul.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2buieqmid.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oiljmdgp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2awayzlqx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2woraomgs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pbhyqrrx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gwydpjzg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2iyjmdrjv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jsgosoxv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2phtlouku.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2lgwcbjlp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zreamkxm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2eokcvfjw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2oyqqohdg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tzretrez.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2keqvuybd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nbwgcnkx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2klplwdnf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uozwtvkc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2huryttyq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rngtflfa.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nbfvevaj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2urcyaztq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ensryqgp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qvmjtrqr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fjyrkwcd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2yqfyiltd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vrkfpopx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mxgsshoc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2brstcszb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2myovfgyj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cmyayzne.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2uulleygc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2woigkrlw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bwxivsos.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2abmqimmo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2nxyoiuxj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xlhwknbh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2aaxjplnt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2osuabcjw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxdnmawi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2clgtgsyc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hwbahawp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qfxtswjr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nvgfwyyl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ayanoams.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2pvcqjvet.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rnixfmwa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lrwkfekn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2irypjjxn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xlblzame.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2gzihigrm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bwdpuqwo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2apmyuzas.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpttrhgb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ropabtli.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xdryetba.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kqzifqxq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2auvpnjjj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zhiyrgve.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qhoklzyu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rswcgtkg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2nwczktya.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2nonhvswv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xwotgfnv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qprbkpfx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dochpnmt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2glbaylym.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2buicixcj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gpyxlxdg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vnspfwsq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2owiqqsjk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zozqfpoy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lpjkjpqw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rygmolck.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkhhxpto.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uhcmkcab.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gmmqcgvv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rvgrwyay.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wfwmohwq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nccsqhel.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ckvmyiet.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vxlpqcef.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2sutjtlzk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vlaldsqo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2arkgaude.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bondetir.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2apxlggvz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pduwzfkq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2iuvwqgru.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cozuyfps.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hmvqxjqt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2gszqhnni.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2funqnwfu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vygulkgl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zfeyeriw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wvmspsoy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ykayvfvy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2imbnkmyp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2bvjnjwka.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2eaupnsaw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iosyoere.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vcjtyytk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zpbifiuy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zcucclxy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iqrkjuhq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rjtucizr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pyqkediq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yqnzzlgi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2agvibodw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2lpdqnguh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ybgvfumq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xoqltece.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xnkekwsq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mtvajesc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ynxmskqc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2tyvbrnqc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jktzpivu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2xyouaoov.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wvojfmys.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lqciqkcp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fitrzkgh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2sxithzeb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jeqmnlmp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mxxmapzw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zuxnkyky.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ecqxctsg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2srjlfpwb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bynmjfxq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vtihtuab.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yjyjvxoy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mekwunek.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2luocigah.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kwpszwnm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2iqivowzu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2lmdvdqak.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2uzmolcnn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2haqbdngx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aeuzwbhl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hejvdfht.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2erpmfhgd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jugattcx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sefacyjr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pymncddu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2upkmixdj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2yzvchgou.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2odqkfatk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uhlfzfqj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hqaosthd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rcjsyyxq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2klgeqncv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saefuylf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lxthxapg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2autbavix.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mgoblepp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fyniovsz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktplslwc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2htlezkkq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ikjxwppr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2thnbycrj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2exihrdui.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2efknjcxi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xltmmdfv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nearuqzj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uqjoiole.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hgfmdmoz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ejbhhleo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2yxlurswi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ibxvtqth.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2sagytmhx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ototyktk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2pobwfiqi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jqjwicrl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ejehxeot.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xjfbhxhf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gdidqmtm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ijovhpcy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2cbgwmbbl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ddwyrtmh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fvywsvwa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2olhuclom.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ifbkvkaj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xhezvpdm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2cysodyvb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xshvbunt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2akerqkld.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jmtfadmz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2otmnfhdj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lkfwcbgy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qscovtqz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2eqbdfhsp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wagxnlhh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dswrfaub.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dvphyifr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ztoxcqod.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2odwfbyri.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nvcqlhvn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sczuoztk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ujzczdhl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qznrybru.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cbvfgovd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uuxivvim.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dgurvorq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vzguhibj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wysductj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dtlxtsbm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xiwhnhmy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ebjrkcpi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2jltbocnf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ziyqmihd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iicpybyv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2staxkpcr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kmzzsfnn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2fwmbayem.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2rwodfsge.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2irimrlcd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qsmxxfdm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2aktmyuxc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2bicffjjv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ituwvwsx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2uikbqbdp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkallrcb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zdyrjcyw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jsexdeaq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rjwrzfuq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lrljlccb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2iqzohgxj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2smnbwyap.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gfiohvfl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kulivohc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rcmwplyf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jykfxkyh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2phsqbeay.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gmhlomtw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2sgdhnzkh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vzkoakez.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jmtszxwk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2eyhmerjh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wbdmrdzt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yvwaqkui.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2knansbkc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2upoxfmyf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnsrnvdz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dztinuxa.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2flqsiqkq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kncolnph.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2qlhizwyi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ccjfdgul.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nexcgcen.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jkdrkmzh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lxefrutv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fzradmlk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ncwatkcw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2kowtrdbf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2heakhopu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2cmkbrnwi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hvoobgpc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cgoviatl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wqkbefsf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2cuhuocbw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dsrrvcya.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tswmmoif.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qkpieqhv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hhetxsph.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoqjlgln.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2cpkydvsn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cxsoduse.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pgojibps.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ydtyaerl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fsrvpmqf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2zakdsdfn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2znjojepo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgvzuype.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qdjqfvrl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tcswefic.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zbditaqu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2puxkrboo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2cucuhzfw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ekptqmqx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ekyvulbo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aajrello.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnqklhkc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ipwuanjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kadboxdt.html


<!-- 参考信息 -->