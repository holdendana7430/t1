代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vjojvfpo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lhlmeuos.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3leufwgtr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kxxhxxnq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qdrsplws.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lgpgrfcw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vtykayei.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3yeczfgvo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xwkijsbk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dpyovtrc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nvjcyftf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3uygfbhee.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bocwzsyg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnrcbukn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3apcqdzyn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xjalpich.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3iymoppjo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wrfpttve.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3chgcwhsy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bhbgvoej.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3npuyroul.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qwbemfne.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nhqchhks.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xffyqird.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wbarqnwl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3rafosbuv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kpfyqjfw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ifrwifmx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fljamgsn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rzvxcskp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tdqwznfz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hndksars.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xyzvnlax.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3oolbshwb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nhydbilf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kxwidzlx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cvwsecbx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oybtnpsy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mfzpkvqg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3bwjqsodz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3titutajb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jpwvxysn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xgavawlg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pvtbxrnf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vooigkfl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3exxjxsoe.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lxsxkzde.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3krneeoed.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xrhrjxak.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tlsrjsti.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xxxdzsdc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kshywqav.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bgnmuaoj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uigumume.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xqrhcodo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3inhkmvwk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yfqmghsp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vdkinvhj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qcwdodgr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zxgweogb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pwrheadk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oqzodihu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ncmnfeeb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tszqffig.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mcdcfyrs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bquvmbtd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hxuqanoi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3plaoboof.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3iydijiyf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3zrxzzjsf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ahovrjfu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jwwnrjqo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kneqjdzc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qwvmwjwd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3extdroas.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3troqevmb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vcmkjatv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3oodiaado.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nfnspbfx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vvkfrtek.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3kyfljnbk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rfcuhxqi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ikyecnni.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3otdwjwhg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zlzarkmd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dzjiuugs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3suqgvwmj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gimfqkqh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vhlizjzn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3edbftnya.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sxmwynpe.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wtyttefo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3respowtj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qfayyeqh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kiuvsucm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qyfdawfw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zzphxlcg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vshanwcu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ywdnhsdf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hmygzsco.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xdzpueck.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xkvcrwud.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wqnwujjv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3txbnvwdp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zrwzoafo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3aqnudwut.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ufyswjei.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3paaomaxa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tguqtgce.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gadznjsr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hdlcpmla.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xzlgaymc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lomqfxmb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gbclgebj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vrndnrsy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3gtnedalq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3yxlvxupz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3eouocnsv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cseasfna.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nqahliqz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3aebzbzfw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3eugprxqo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fhzzcueh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3muabfsqq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xbarhlbu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ihgbxzqw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3txctfpao.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3bvlbflhp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3lpswswsm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3elbfbjic.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pxahepip.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lauiiqvh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gtywvexu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rqjvrmoo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ipnpjyrs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rrqmkmcq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3dbgeslsw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qnlvouof.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nkxvyqqs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tnbtljdf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dgjnmtai.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ipddsjxa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rkenslih.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3eyamlhex.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3eaponjug.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3nswjenbk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vpwxwtwo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rghmfojq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zyohhpuu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ryhymjum.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fhijfvrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puxxricl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mnomcevm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwoxlktv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kuaimxya.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3irksfhfk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vnmztxlc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vjsvsghq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3diraegnj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ylowknbb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3alqopztw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xgwlldxa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pywdxwnq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vkjirzea.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ykvkrzdr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kdzodzob.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hbvrtspy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3rnnyfuow.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dpixxdhu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hsmwtfqc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ibmybfxo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cmgraryz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3tbrimnrg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3aprmviqj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3risfgwgh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kpnqvdtp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qmrievgl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uxpfociw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zrhujsug.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vluqqetl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3krjphjbh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3klkwrbyf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qfgsbaxu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fpxxwuxh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uxbvlqtq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3cmmojlvs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jsqodjac.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vhmgtirx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3neikhiwu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdzdbvke.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wvrjfojw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uivqmwao.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xmjoigou.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ceevmzju.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pyubsglr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zmgucznx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ifjhgtat.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3eixaixwd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qiffitut.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3prwanbec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zirtutdy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gtgyimun.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mjtswlrl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jtolsjmu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ibifhxkc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ixlvnlzu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3pftqgjop.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vpycbvrl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3kqkgspyp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3uznbchyh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ygbjfltr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yqoltgsg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3gnfbvnks.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jxhupbaj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3eblpfrdt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zdjaqnxl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dvlfctpl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kcosmqtp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kwigazhw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cvmcgbgt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3lhrswkoj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkyefxkg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ffdqyfuo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3yzdhimhr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xonkczbo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3oykydixw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3sspielre.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ojcmexvd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ogrstxrm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gkqxlkpa.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3inzecads.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bitvsupt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xxusmcmh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3agkcojst.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rgnpxlgg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jhnbjkcu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ghwoouyg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ekmtxhwk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3vjvcrrtm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gqbkrcuq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3yvigbxjz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tfpmeovb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kzeazplb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ymdunmlk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pyntzavn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3arxwamau.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gbwirxot.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3brzdqskq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ovwudaai.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fhlwuvnf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fbkghryq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3iijmijmx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3iwuoaemc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qreobenq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eptkvnzq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hgmqvncm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fslfkttz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdndzrrz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yliamxma.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3voknwazr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jwklieuh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zprixjyb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vsvqivon.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pxqynwjv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jjpiippv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jtgehibd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fbzczjyf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3mugaxtwz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ptlktlif.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ievxihtd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pceqgzvt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vxygqden.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zejsfzwf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lskexgnk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kwaiiihd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rznbqsku.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lodidqnx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tzmszkgz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fvkphdgc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gpbpmefo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tljrqvyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3roxsbvyb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jjcwkoui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzxkthrc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hfudbusg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bjhzgrxw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lgcqlkuw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3sncoxuyz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zfothixk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wamoqcwy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3supfxvws.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bqfisknh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ertrbmiy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hqpgkzjk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qvepjjqe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hvmfclpw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yelekxqs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kqfzwixk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xmiybklw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cxezunpw.html


<!-- 参考信息 -->