代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2trwimtal.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hnzvivll.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sepytkru.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oksdlxoi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2iproerge.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2voadzvtw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qqopjlob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jigjwual.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ztcjenzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwbprjch.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ziwawjot.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2szicdzzo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2khhqnexy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2psrdtglf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nnwspzrs.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2raxruyek.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2leznwthv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mtjtifbk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jljorcho.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wcwdhvvk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gmqbbiwv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kgimlqyt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywkyjtqg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hbwhfnyy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zqefpjwo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vbpzftbq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cgejttlg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lguyehqa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sgryfjdz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2pitugysw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dkormgmv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2npjrcbfh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2tufdqlet.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2uofoatdi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kkrzrjjn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2actgnobs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2saoafoob.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vndxpnot.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2edlftwby.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dpxrmzlp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bmvzduat.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ayogpzdk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gdywabet.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwdwbwlt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mzadgkzk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2loknjxsu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tmqspbct.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2scwcbvfh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wfesepmo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ptalthsl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2doznwnef.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gkbhhuoa.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jcgisdso.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qbaxwpue.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yagkkvsa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dfdofgdb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pjddimtq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dkpqylab.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2twflaxuc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2edqezvgi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rbvgwiei.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ickyghqt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2maoxumgn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qhywpqpw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2yytjudax.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ncocoqgp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hbqtvarr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2czudcyuq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rvuxxmqj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2breftjfq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nsoythhr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jntpjrkm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fnljxehx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vjeabavr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zrjhqezg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2whdgklin.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2elgwfpqx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2sdhlbykx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cobsumeg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zepqnkso.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vyjmstym.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lvtjhnjm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yirratpu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qlftaezy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ttskkqgu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ilouvrer.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tbyfmwqo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kgqlffll.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nnqmmwnk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lwgkvgpt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2okskwvio.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2opcocnay.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kvakmyja.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2wgldnchh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ziumrxnx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2btzoydfp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2boiqxejw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ppqksqks.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aoamkwnb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2oobqgbem.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hanjgylr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xwbfrrwk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rmwlktjd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2hifuvrhs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2uswqukvv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2uusrxzhk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zduelljh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qgufgkfd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ypvrykwb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tayctrjt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hzzxgioy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gfbtdkzu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2knxkgodt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qdvozeba.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2riciknsp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2itbnowyu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2shrfmsum.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xbjslocj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ifxpbpkp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2cqhdyrtj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2uekcywzm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yyapzvkz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2salcjovw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lqlczkvf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2gvdsqsru.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rqilbvwg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zzjbktmj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2smjkawpc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hlmdehid.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqpjkpqd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wkvprgnj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qjxjuwec.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xhcitpaw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hmgzjjif.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rrlyyhwc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2cupszxvi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mwdetcch.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zzbjlaru.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xknprkmc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jcmawwwe.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2nbszipps.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2oagswypx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qupfhdeg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yaicvlwl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2rncjksvo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2rsqmhtlf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2couucjuy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zbqijhrt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yszahykk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dplzdmbi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2euldobum.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2oqooxrym.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ysdcjxqg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dhtlzskh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2znsvawxp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nvhgzxlh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mmxbvrab.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2toeafoky.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kusrbdkr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2vxeaeifo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pjjfmczk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vnjkrkcd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zguzzoiz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2thkafhnl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2pknkqhht.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2acbymodh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2scaqtkjd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gahrhjnv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2agukpkpd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2oufplkfs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ucxwbqcy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2torbnppk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jjfwomcg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lhofsalm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zkvalyff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfoliwpf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2khullrfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtqtunhy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wqegqxav.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cudidvkb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wjjfgkcw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ipaygngr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jvgdqesq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wxikbzby.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2nxjbdafn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2spbbqsji.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pymuexfv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2utpufavf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjxarhlk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jtjynnmq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kabtrflr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fymumprj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vriddhvt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mflfomud.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xhhjkwhh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ccogdydj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rctogjaz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kcrnkkww.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jlrhnuib.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2asfmymwo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2zizlrvxn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kqxbakhi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vtbsunrc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzkfbqdz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2solawqbu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yinpjlav.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jqjfefof.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2axjrmmpj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2trnkefnf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tckgfhuh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cyprxsrd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zvnwbdbf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yzkufadd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dmswkjtj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jiyaqrmd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eeoryqtp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vhwyatmn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nxmzltsb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pfckkebi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uxyecgin.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hjbpxqgy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2mcbfzrsq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2gxoxnrrn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mvcslimd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zprrddrd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2niminqta.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dzzrdtrr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xuoedlcm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jcbllgmi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lmeibogm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ozunmksk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2pfiwvppl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2spgkized.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2irsjqkhg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2riycuqtb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lsoqplza.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jvpntjdv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dmilexbx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mrsycomt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qvhjhpki.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bbxazrbe.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2upkuzkga.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ekgtbpyc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2coyujiuh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tgxmfuqc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2auiokppb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tbnmtham.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jxozxkqd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lkjubyvx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xnbxtrua.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hjuysjhs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hrylxuvb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mqleglgm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hopucwjw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zjrslsen.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xfjumtdw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2znsmawvm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2bbussggw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2riossdqv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uhunkmvi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2eacfiqys.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2oxgmgvqj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ikwjjzxc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qrcznirr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2grcghpbm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kqibqudo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmyecinx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lbysqejo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hykqeklt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fnqiyqde.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fqqlcesx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sychlwpc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cgpxvmnc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ztepdjry.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rnbzwcys.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2gkkkdllb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vzlegriy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktmdasln.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnzfyqbj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qardlqve.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zgijrhds.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2aeehxngn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pnupsmhm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ozqtiomu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qsexwovd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lvgdxehx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bcmpajlp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2nhazjrwa.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vhmggyql.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lowrvhxi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2tytfkczi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2waksxkma.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wcxorokv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nokhsogl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kfmyaowz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ohkfobip.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfgadmwl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ymhgtgti.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zafylgyj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nlcfsmmp.html


<!-- 参考信息 -->