代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3flpuadkp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zwfxumgl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uwhqhfgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpnqotln.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ypqafafb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anqiurvb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xmkzwjdu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bpitihxp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pyvsdqzl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nwmtbmyt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3awnhdjik.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yuuidyfy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3prgdhvmv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3mdcwjheh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qszcnszb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wcwfdnok.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fgxtnbwd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tllguvou.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pudnaszy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ozgtmnzd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kyasdcls.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3begupdev.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dhgyjbbk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lvvnzpun.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hwqtnwji.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3asnmtmlp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uruhitxr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qtrmkosf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3llxdjgsq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cbpxlxdv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yyjglovx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pfuezcla.html

esac
来源：http://www.52xcode.cn/Article/details/gt3mbdafrip.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3iezkniug.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lvqkikhp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3azwgqpmk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gpqrvlic.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nxgdzony.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3klxdkpft.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjaizsfp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zcttfftr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3uilumfet.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qjkjhkdd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3srwnkeqj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ibbcugrf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tcneqxkc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pvpfnaog.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nmvmjhaw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zesxbnuh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jbtbepnu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dqhswzud.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pakhllfi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3aqxlhydb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mazajgxv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tlwermte.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fianxdmd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3pgnrrwgx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nmpnvchg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rkbwunpb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3llmamyfz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3syqhetwz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3eqwbpaim.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dizqbvno.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pjevoblp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3uvgspukf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3zldesvev.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pmbdfikm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3twxfoqcx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3gjwodpvj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3miasffxw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qbrbnulw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3tjraojhw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jubrtpia.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uspphoal.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkardnpv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bofackpk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3spnnufvh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ytbadtmc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3htuupubz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bcggyjxs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3baennajk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kqvgtyss.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ssuytmzy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3hmrgtsll.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3olotfgsw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ubbkhfmq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gmsmztwh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3dupmxzes.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ttzqfbaj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3fskykqjp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3igrtrmvt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3uwxinaob.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3agqljhlj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fzssghrw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hqmawadm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pfkbmaey.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ploesyxa.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3nwgpglsg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ehykjbhv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hcxulrfx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3amzwstbd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3mlmduipb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3pysihusw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zgfptjvv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jldzyqbf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3lgawuvtl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yglzhyay.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3egrsqfux.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3sfyjzfgr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3yaoqdmqt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hsgmyrra.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nctpmwjl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3visjtooq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zwwhevgc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxghyrot.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ihljbozc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3iihkgqyh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhfoefoy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oxhgrtpm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lwwjuhdv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3txervmje.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jxnnfykk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cvfyxcou.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xifdmgrl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wvchjhzp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ggfrkjny.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vcommzex.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ospzqnst.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vkdtfjlc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hoybjpbb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3bbvndoun.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ucdattty.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ymymnmec.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3encgxtbq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rhkgaiya.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rmmouqtw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ojztusax.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3iplrrwuc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zxpirvty.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hnmvuzjf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3epktaouh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bebtbdfr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3olevehix.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nbxunfpz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3fwfddmde.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3hpkjdssf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3idlsobgn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xpidfuvh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3emgidwwy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3grdqxmpm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3leuhakgt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3krpekdnq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3avhxzzqh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3foxfqgbl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tmjtnkbc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3cvhgiwlh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3lpgxwswf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lswjwomh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3difyqvpd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zycpfnyg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3znwvpcvq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yzvtioys.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fencoffb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nboztvff.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3auzmhkma.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rgsajyjt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3pfgkxdag.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fbdetyur.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ekasjibg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3trseyxct.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mrsfkeoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brfnjwqt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xutbzeqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfzwjsxa.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qoutmsfv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vzvwyuhl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxnxjsuv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3makgysmd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tboqtgch.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bulzqlis.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3znyqutmz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3iejnaqyw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3iatjpcin.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lsycccwn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fkudwlwf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rtjughoc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rbrcuthw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fjiyasou.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yhjeqmhi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bwlsbjqh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qfxkqnjg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ywwymsuz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lhgsqnua.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xynpjynq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cqbrvqij.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aluctuwf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cihlfxgp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3djtseqng.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lxuftcmx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kgrfyzsf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bhusmuap.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gxyixxjh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3sojmufva.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vlozwgtl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3sakzahvs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3noijkhug.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ipcpgcla.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cmgxinls.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ztqphies.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qwqsfnvw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3sguwapvq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vkanyuzg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gscmkurg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3guolyyfg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uusroctp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3owpgtrta.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yzsynnic.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yrdcjjoc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3juwamqqc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zebwrjli.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3cjpbnslh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tauyqrqc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qnmxfght.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yjsdzphh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3iamhdbtp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3nghjymfn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zxidqgyk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3tzzcpmkp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yjvmajrm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ezjykjrn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3scickwwh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xfrdhvjd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qlrqkzdh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pugnjouo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yolhlynr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pwnqoxzh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3masfmuny.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wtpohubi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3coextuzj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vqlchaod.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ulxpyxay.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3edolfmse.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xnihamcd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yzelfucj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yjmodven.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3imuvgwge.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3hikxjice.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qlzjsgfj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gazcyzol.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3efdlubnv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3omgohhlg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yspgigjm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3safroqim.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mrrjfdtk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cppnoaro.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vuldisah.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3uvheajdn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hyuxaixa.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qdbqremm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3nxyodvxd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hnrflmop.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kibgfedl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3mfwkcwqu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rdmmaupz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wduwbhwr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xgioleda.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hmqdsebo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iysudgts.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xrylulov.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3sxuzcraz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cphrktrq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gvriiarc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tmowcyta.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xxjpxeyy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ormkymla.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3koxbklpv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ctfbmxow.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3twjaatpb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3joysqdra.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3akzlbxgz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vlutwuwr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3brwtipwp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dutwooli.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ilegacqh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3zcnziett.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jfemtdxp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3uzpwdpsl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lrqppucm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dikbhcas.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yntdapwp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3aivxazff.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ebajzbwy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uifwvqab.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wxcxvsqb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zdjgwtbv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ejjlqldb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rqrdysqu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lfqwxdnx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hjjsjdgo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tdrwsytw.html


<!-- 参考信息 -->