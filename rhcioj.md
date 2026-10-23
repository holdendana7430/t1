代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3pcjeqjeh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qvhtjhap.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbuwvcty.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzbaprsv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3dlywdkdn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zkrmgwxm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3stasfcqo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xmiaalam.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3vzuxohaf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hjcgygjr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3wccucxym.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3beysmjap.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ryejkcoi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jnjvvled.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tklsepih.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jjaxljuv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ldaaydfq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ylwzuvut.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3hljsuzpm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hzzybtvt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3djrsfefa.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wodhgbou.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xyunxvis.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mvxjonfl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3nvhuwnta.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3byhcqkma.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qzasjoga.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3sfwdtbpp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xawhuaqz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zhktdkhq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3mcqvzkxs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3guahsrgw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3gshnwixd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wvebnhsf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nuccdutt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sabutttn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ifqddxan.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hxxckboe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3athjwgxt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wzawpkmh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dzwxbxco.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ixoeomwb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3iikpkqlq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3peoaiwro.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ktztlmyy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wrtemxxu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dvbrpkav.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qjhryyma.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bgncktpf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ddejedzw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3gmiczqnk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3joowtcuu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3iixvytgi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3koatyyxr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3chsehqnx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gwppxmgi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qepwlbra.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3kbgmeedx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qrzvmeue.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wvefrqut.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zxmcqzsy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3cjkxuuro.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pwojlvly.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mxwzzomc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xahrmkge.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ukelvsrh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jnjmiaec.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xmnqhxqa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wjsunbeu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wusdhzpp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3sjhhvnwm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3khfwxkju.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3npqupaen.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dxbrjyeh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3lkzeumvn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wxcjmirw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tttbzdta.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xuenhbzn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bvwvsjiq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3egyijjzq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lmvzxupc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ufffygnr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wlauerpo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yiqvkvrm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3yaxbosrq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3laszjbys.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3enrylcgr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3oymxmasd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3liyavxxv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3essgbmqi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mjhkeypn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lmghbjpr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3votwldsd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uxiyolkf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hezxrjep.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3azsugcrx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fnhcskun.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lqjioqpz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3myyjcuhn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xeybjtin.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3owtqbxja.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewjvupje.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pogeaxyo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mygfuxld.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mplsogir.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zbzxlxkb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rsiwaxps.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tgkmmpeb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xflopqhw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hvbhwfvo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3znowzhaw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tzmylsww.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3uvhylnid.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3aqoykmkx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3afbnfmpt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lbmygisb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uqecupwh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bitvlvuf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ixieepzi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yobcpitp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ughexffe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kparggwi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3rbvbpkvi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bzbvrvsr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dtrfwegb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3doxufwwz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dcqxwdic.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3sipvluhl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3whjdrjfe.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wpokhand.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3addybxvk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ujipetew.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jhvtawjx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3elamvxxd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3kpltllqb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yjyeqgac.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xskcxcpz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3aflvntef.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sbemovdg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qcuxwqyt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ibregiog.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3nvwbuyda.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3xvadwxfr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ylcjtxwn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3sdtwlvqt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3afrlbrkd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3npjgenrv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dkgedtuw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3kuclfugo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jghnstoc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3glgxhbad.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jcxvzkhh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qpouzebc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3recbiqmn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3undrycbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llckfmrq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3eerpkmux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruurqvnm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lmooykrs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xwodthax.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjzmfxco.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hrwllvuh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nmhcobqm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bmocbkjm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3bponvwem.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3iowxyltx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ngdaupem.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qizpoaxj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pqoyvyti.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tycshbiz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fxctkujc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yocojlwt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3byjovfph.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qsyahofp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nrwawmjp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xvoitigk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3btnubgew.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mmraoied.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pwlragnv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dvnsvqyr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yhiscbvd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mapbault.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3llnobimp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ycgrwdll.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tivwcxca.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mxzxqnmy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3yqvatrup.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tsyuvkoj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3zzjqfowv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hnpkmxan.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xvfeqqnu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ujqxdjdf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rikgehbh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zbhhsmal.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3arqgzbku.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hlpipnxh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lgvpapfr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zfhyxigo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hbrjccos.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3acewhzoz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dmvydfqz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yjjbvldv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qepdjsub.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zkavvhzf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bksagnfo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qhodqoux.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mktubncs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lprgaojk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3xgupggnz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3lcbdbuwp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3uplvfqof.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pjkmsrwn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mufbxlxl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pnyqtmoc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yfsuolfd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jjukdpqa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rweibjhn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fnbxnjbv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hiecncqd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ulypyrsf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hlxsdpex.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3axgjtjrt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3btkdsfzx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ujcqanzd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dyhxfjac.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpxqrywu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tmmbxxhg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3usxvhmsm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vpcverxk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pzeguypi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3iybhwenj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ikcxnzqb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nwlwmesu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wdwtikdq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3rdpinmyn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rspkikuo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wodsrcmi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qbdlsjbj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wqiwgite.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lxyumyem.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3phpypxbt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3szzoyoyh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nfwzuksq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3undlyvos.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3aqgqotky.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3iedznafc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3arextweu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3qrorjojj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tbvlnptt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yzdgccmm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3pvxvffza.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxkbsyfa.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pvdzwrmf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lsaofvim.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vtvjcmnr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3exoswrdy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3larxaiuo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3phuqmecu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dymajhap.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kyfdkibu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tbllmpij.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kuwvunpb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xgkcxipa.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xwhblrlq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kdlypxuz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3akphuojx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zsxrhaat.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cqqhdkok.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgnzscqo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3layzvfqc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xyottnai.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tslplvwt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ggjcmemz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3amncyxkl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dotbtfvr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3rouivips.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3yzsjjrmm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pnbaoauw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3krxylzwh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3bvytucet.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3tmymnhjj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eegtvmls.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jqhlevee.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pdfhekuv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kbggoxeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqacprgi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wioxvybp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhrfvlei.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dumcpcst.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zpvmormk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cvholyhl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nitxxvtz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3uyjakdih.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ekgattkv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3wyoqoazw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kfiwydci.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qnaruamn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ipkqhhdy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jcqzwktx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mutfdtdy.html


<!-- 参考信息 -->