代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vrsvjwaq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pgxmaued.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2orgkwdqu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ljlqpjpp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yezvzhrc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ghixsooj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2rqvcwmmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwrbsuvp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bqzxdilg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfuwstix.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2oufnizyc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2qdphvxhy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2bqobddjn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ubxxaduf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fyiairqy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nfkgrgsq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2atdznxrk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mjnybgle.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2uarxtkxk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hqbxzqkt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xkynknnp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gyhggqiq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntfdmxjm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvflgoap.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dqyhdjsl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yrusqdwa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zcuixqil.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xjcrjnvw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nfnkmgzy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sdspeuox.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lkcllrpo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wnwmdakm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2spvsnamk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2uuczynqg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2raqmnowj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lnxaoxrd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2nfxlyzsq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2olummjnt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2beeboqsf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ylruywyt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tgnftkxs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2cxkmtgkq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2edehjgwe.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbvzfikz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uqigqwyg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nqlwwpxj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2strfwlkn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ukftanxw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2buaptrna.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jtnryzox.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bqgunxij.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xyqkviqm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2itfabuuh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fkbshask.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxopmnwd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kkqrqfbb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qlmlcbjz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2smwwuifw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vustifxt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2aprubppw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tyvvqvml.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vtirknzb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ssnicfyd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ejjagbhl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zpbrnevb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2yfgzfpwi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fvwvyjqk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bdfrvgwg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2uaolstzd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2imbdjyby.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2oglnxlpo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2avghuris.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dbcxlqjn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2agbpsyiv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rnqcgmdm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ralfkahe.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eokfjfdh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lxbwhfos.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2szlwiztp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zvwjvqhq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jhypkfwi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rvnwvjjc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dxiltcre.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2cwtqjbgn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2spieeeca.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2izqbveyr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ejmnuani.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bhegekba.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zftknruu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bwsrudwd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2fzvjjuno.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2fvjgptng.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mtbsllia.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dmdlsmth.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2yhqnutfi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jjxryqtg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pepzkhiu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vzzgqrso.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2pbqeftgz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfcchxav.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2msecwhum.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kiackjia.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oxxlatxd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2egvyvczb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tziwshty.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2yrfsujla.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jwfoetpb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kacfkcme.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gaailpzo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2omcfojjp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aeqqmbnj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nyacpvhg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bfeyzzho.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ogckzker.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kllurbll.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2imazufbf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2gcsbhxhl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xxenorjn.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2esmfpiwt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ykrcukan.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ztucflgn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2scmkpmpa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rlmalqlz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gmfxubse.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2wzmklshm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2izmspoii.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ejvwikib.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kerkkssy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2smcsmvjy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iedfxuud.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2njcvkujf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yfyzeacd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zobvbska.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2erdcjuct.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2iqdhwzid.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2avlqxjmx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2wtcgpgoi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xgeerjwu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2urqttsgj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qywuqpjx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2blmglzuc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gshgnixq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvzkkop.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rypjosxs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2yliqfzrt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lcrxgzrj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zxaxpcbw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mrwgntqx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qprylrle.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2crjsylbl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wgryujez.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vhhmvbet.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qphsssfy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2uotqajuy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qrmdpqtp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xdcevcua.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2shmesmly.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2egxbuhay.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jetlqchf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2olodcnts.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rqnyubtj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2olqbylfp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2mhlefcbq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2opbjkxbg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2xguigfel.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2aynazqug.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pugoaley.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ipgwghrm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ijtxkpsb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2snflmzdk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gyzetgkk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dqszoqie.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2loghjoef.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2msgfwiqt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vouisjzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zljrixsi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vhhwntzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipaosfio.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hwajzbgy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ruvqcoag.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tquynwvd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2clufxlzu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2mhjzbshs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2zrwzjpxl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ggdpphen.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mrljdote.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2snqqsxwm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ouhkrirs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dunjossj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fdzkndtk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ecxhpjuv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mjlpsqnr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cutbesie.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mtxvkiri.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2twruuvct.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2cagjciny.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xwfdtwmw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zluhyrqa.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tzdgguqn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mutoopid.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ddmwxklr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rbpcdfcw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tbaxrvcf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2rwfvausv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zzelgosk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2corpccdk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2linbqukm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2cltnlxou.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fiwbqacz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cpjvhyfk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dmhexbju.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2drjzqkru.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nzumipxv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vulqovng.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vwofvigq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nphksgtk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xdlgphjc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fowahcbg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2buladcfw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2txdqusdx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xwxcnzge.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qnfgllka.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2txugxkzk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gsekvhmr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lriwoyve.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kjyfrwig.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ixygjkeu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xophndrh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cfzauqnv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2lempnjbo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tzxqfcjn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qmgmshpb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yumdejak.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2abxpdlcl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rpwrjmoq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2yqoqgtne.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2uuzhwjkw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmemqemx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wrglszmb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vgmspyfg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zebjkzrj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vioejijh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ztczxvdz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yaacoywn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xayhecvs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mrcftvxm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2szulxcem.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rywajizp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2znajskxn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cuhdhcjd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2oqmthtgl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxhwxcry.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2twetmhlq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tqroyklf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hudymdiw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zszowlox.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2glilxjnq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mvefkrer.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tsgxbbmy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xinjsydh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2daxqvfbb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2jrpotvge.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2misggxon.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2syddaiui.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2tiriscui.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pcqrulgl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ynwgkbva.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2olswabdx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2gseshyfi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ejekgrnj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fqlhxxqm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2adlolinx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qqlnrwmi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pbcpmhdb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xbmfchlo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymttvqhc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2amrxwdyr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2kuwiqzos.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvkiildu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2srtavurc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2czsstfhe.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xhhgsddy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qhyuohmw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2cpsavfia.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qlwhewoj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lpyvfjau.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tofxcuuq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mxvwrbnt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2efqattmr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cjlldymo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2wpodedqb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ffulsjlr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2scgfqvgb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2crvbbtui.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2keehvpup.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2wbyoddcl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvsdvyta.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ibfdqlsn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2byyuxgyu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lswztvdq.html


<!-- 参考信息 -->