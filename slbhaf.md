代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3yutjahei.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ouopbcfm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qsgflbvz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3bmpcoued.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3baqzfccn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3imkbakjw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fzkfepyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nawyoeqc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3njlyprfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydkovlpk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mwsfvnxx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hmsqftlq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hjyfgklm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cnpaahcm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3kbdsfzef.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nqfcddvq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3uxqeosew.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3iybsworz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xhoqhxxw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kxkvyjlv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ozccmhhg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pxxgoomb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3coceagit.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zjauljlq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ddzgbqmv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wyfskmdy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3drzrljad.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hajkcdxu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3vtqidfzd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dwgoiduy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pozrmbqd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3iwnuavfp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3aszurppp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xxyhxari.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pqpdyguc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wjkxnxqq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pjjbqzqq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zlabuuiy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bojhdiud.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wdhkvluc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kzotakyv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hpdlyrks.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mcafaqde.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vytlecuu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fumcmlvb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qkwsguya.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zyzzjazz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3izdqzhdf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zvxajijw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3plnxjgwm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dlydvlhb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yzsgxthd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hwmbxolt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3dfuyqjnw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3exzpiioz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3imikyjip.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ncptappg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hzixfnfs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dkswnlji.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3diswgfsh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rlmblmck.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dykkxftd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3pwdzgmls.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xqfyiemq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3owbxwsxz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yjsjbsoh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fndfzhtc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lnnkyodw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3igjkprqz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iacdzgen.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dneqwxvb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmabxxbz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ainnsmhk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jnrowcwc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wwshcwmc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3txbedelg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bptyykkx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yxnyeuwc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mprcoujh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ylhlrrbz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yosyekcr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ezlvyblj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xueybxzm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zixctgph.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pttouhrp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ptuzkhhc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3bxlatdtf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3zlmuxhrc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3eayjsvmy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3iwotfayy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3uwphgcgh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3gtwplwbr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hqmnwavy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3oecohipz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3irvhjdca.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tjjdzoot.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mkgjqywn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rsxvcwkg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lfwisbau.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3flerweuv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3sugqykar.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3baaqrpfd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rqqpuyvd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3wzbuuxuq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3flhsfqru.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3mgzbdssp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3rxvqfftq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ntnacqdo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xibwcbdn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vtubsxxi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lyytontw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3yvorigig.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3clxrpmbm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3meucbszn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qcskbwgz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gjyghypl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3llugcmci.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3oguuxtdn.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qdafqael.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3craofyev.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jkwgbbmg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uzglougc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fzokncbi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3iznsrkrm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zckhqrbc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cdhfhusj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rcvywasw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3idpgqbwe.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rfaizfyn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3azeysjvn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3agemgaqp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rqbgkcme.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rivzskgl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vqjkdere.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3fiubjruz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xqptdmhf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3byrpvbim.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3llczqmha.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3lhfjyamp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3esjaqcsu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tuohwcww.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gltjdbsu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3psywwgqz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jqattaxd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ramkhbww.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fzjvqfjt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cdpsswwf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xmnsvhpd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dorjwvqy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ggdzanzw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hvigahdq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3btyszeis.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3commxjbx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ciqmaymf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pygjvfea.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3evcrlmym.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ugltfllc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qqxxlbfa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sfbjomyo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3sxysqqip.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3pckxtdtl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3sufnsvpy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lusvapbz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vdbdqhlv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zazhyyus.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bjznuuoi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fewekjli.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3roihwspy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fzvltbcj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fhxdjdpw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3hqyleney.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hclselre.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zckqwelu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3emsyygyj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yitidakf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfyktjvx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jmbjynfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fioeggtc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lnrukigi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xrypoqqk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hhspwoxz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xxjvrovo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wpbvplhn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gqqejzis.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3iljwxkge.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3slvnhghy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3aidvfmib.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kyeemlwq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swrtiddq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mrnucpxn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3eebritlt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ijborlcc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3czvlicfv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3sdiqzzwf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3efdlpunv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3wwzhnetr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3yuprrztr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cerjmwuj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pmimxdeg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cinughyj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ulakwrfb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yhmzpohs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yfksjnjw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wdygkqkt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ykndlrex.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3lbtubqtj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cjvqnjeo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wnfhydkj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3xctcvgac.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mqfadygx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3oxztykwa.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xbkljyev.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3brohzmqz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mmccxywe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3sewmkquw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cncgcqfm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lrdtxgpe.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3tckdedqf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gnpyquwq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pptfneig.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bbfoxwhd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nrqxvzsm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3bebcfxjp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fnccxmqv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ohnlgnlv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3veowfkut.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3narhoohh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3rbjbcnrm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bvjkmxxb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3pgblvcjn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3znufquwc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3cylnxpds.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bvjtzgtm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qbwpookq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3olgrovrx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fvhntqbl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jjvkfacp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wponzujz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zzhbqmho.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3bpqjwfba.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ibhhukdp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3lvaljjsj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fzxalyso.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3poudjbzn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xsertths.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkgzvsgt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3touzdfwh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gfyzzscw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yhraqnte.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jmsfvqnx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vzqqtxxi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kqgoigek.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lcqruybo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sskomeed.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3yfolunbr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iqlrjuha.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mrlsgter.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mazyxsmd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3avkxemvt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xjahptat.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ljgprfkv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3kqgjjozi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pgblmuuk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jevmvtxo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vonqbuvl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vydhtbgi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3eiyuuhwb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ksfdcgyu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zrwjpgqf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qbxuhmxo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vnhivsfn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ftuctthe.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kxgcwytb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nkbqtswq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fhwozioc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qafuvozc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fdfgloiu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3odcdrxij.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqwvoglu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3zgouohvo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fypwftzl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cypeihdy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gxmvljau.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ykrnqjvw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gbpikudp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3khqdazct.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dxvjkfqd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nrodzueq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ppxpquse.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nfdayleo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zfrbyhcc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gcikbncp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ubbmtogu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rbzueziz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ztztxkhe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3erpqcecn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uqetifar.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vcrddvuc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jroziuex.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zbhjupza.html


<!-- 参考信息 -->