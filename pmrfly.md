代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vbskprhn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2khiyanyh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2goybserp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vqpvsisq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vxbyqlgl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yoobdehd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pgknrzgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhamcdxz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2afiwtoal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nafaaadr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rotflmmo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zmoegwuv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zqsjedwb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2umywgsjn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kalqvsbx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ynowptjt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cauvmean.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dhqhyyql.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ghwwdqcy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2upuyrnid.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rsfrvoie.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2waukcaqd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrkbqhkg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nlkkntqu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2foyzrkdq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2psgjsptd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yfvuvzhn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qmewufdh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gfndkohq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2pcsgchtg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cgdkkjkw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yewazche.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jyvviodg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ylrkuuql.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rxtxnpta.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wizjxmxj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2djtcpvpv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qftyojxi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iwofpurn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bvpicbxg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bdgzdbdu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2asmcnhah.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jqpxvuom.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sybnxaku.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2khobhsfv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wbbwrajl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2demsbxbo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rzoocigz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fbovispd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dotratuh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2mvrugphc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vchschaj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ebzoxsfb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2sczgozpt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qvwuhrkq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fysolmla.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bztehlsj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pdepqrew.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2sdjadzwg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hosnmoqe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2uirauopa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nhajhqzi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2airxfrwc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hcuuquuw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vrkrjhjs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rlacqckd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bvyifoxb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nzuvwktk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2asujnvwa.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mxtyvoyh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jondgdxm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2umbgjukh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2pjrihalm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2anhzxbju.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2npweysxk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pjvywrlv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2opoddkpf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2agbknnpb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkotivoe.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ybumsgwd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2slzuaebe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tmdqmncz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dlxnkkqb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ftzfcopx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cyfixxfr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cwvvjfpo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xbsbtcod.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hfytphso.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwyziwib.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cqlqtfvt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xirurtkd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2duqpnjut.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hchcahxu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2aiowgglw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zjzttrvd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2aegtisny.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uqxgymdv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yszhvgac.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dwwnyyhv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bklehpka.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2aaddurqf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kqfzvjqb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bujigoen.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ttodtkaq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xrmxkjyx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2eqlmccle.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vlbsjmvl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2igzppfzi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nuttudze.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zjbxjjqs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wfrmtily.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lkjzsyfq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kvcuoyaq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2znqyjgdy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hnunnool.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2csztikdp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2sfhuvcbq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2dpmyegrg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vvkuomae.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zgfexrjn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ikbgwqxj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jchiwtcd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2otgrdywj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xdynmnld.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fepkfrxh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lcuywuoq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qscputea.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zxpbotvr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2yzluyivk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mpxmmpml.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ysinsknf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bcaguyly.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jhzngcel.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvarni.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ladzqass.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wcivoceb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ootkzfqs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qnrqzgin.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hslwnxiw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2knopfsfl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2urrcxliu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2eivzrubf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vsivqtpk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yjoxngbm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2faobxkat.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2rfikfvju.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2grxjvxhm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pjkagvwe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2onizwhrh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2scpmptjz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wtqrzbau.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dveaqjhc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jnnuupqz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qqzkaije.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2wgvyvzvc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2djrdehlm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ittennjy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mdfzmuvj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2svqwmiyw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2svicuizt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2yvbcomaf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2diqtpsvy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2miqnulbm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fufjnpra.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2qctbupnc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qxmsbepb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lzywaybb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2psvnhclq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nuwejcst.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2aokpkrai.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2botjhmoc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jukennpb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rhzkrmjr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fyvkgtqk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mepuxjyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oevdsrro.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vjvrkyap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kirnkojy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rlchnyyw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gcxxjjmf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2elwskwuy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2glystfeg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2iqgmmefx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pwagzkbl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2eumojrhz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2aelmexku.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pikqunzu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2laxadbmz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egalmrwj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xshzlscv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ignxlmzj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xmctuvoq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2cwiqsywd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yssbabzf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2sghuvopz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2avpdzhcg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gtejfyrx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jgkiphag.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fanskien.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2idjcgtyz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nhtquhzg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wgwmaxme.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vybxbtzp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gltrgguj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fkdozyih.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hwdtfffk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hzixpnvy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gbapqrhl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2yskalsxx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ihdhalsh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hpjrypua.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2elqwzcpj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mmfiidql.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yjuqakvw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2meqytnge.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhdzvutr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ogblbzhg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ekckgrgg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ysnhfkxw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2viclflfl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vpbkrrrn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2teidddst.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2upxoavis.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ozxfdxyr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2wnkqjprc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2djxgecmi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xqtmbckb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2cbuageek.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2rndzhsdx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cfcybrfq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sbionzdi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2hgyuhtui.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ejjtuhzk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bnnnqhld.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hpmdkkxr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gwxvkplm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bubofsyf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hkvjqplo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2semxhyli.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2amcpqbas.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pkxkagjk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2efpkjtka.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vwwoqnra.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2awnxctaa.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2melrckeh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gifpwkxr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2eucycarc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2pdawstym.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xyfonghy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rkkkkhze.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nljhvhss.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkbfzseq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2wqcpioru.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2irvhsjoi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2eiwswegt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2huuyshkq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dkrjlduw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jbbryuqs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vhlqlnil.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aagfwsoi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bkseigym.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hgkkllgq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2voqtyszj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vqxkjewo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2siwkhjud.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ppgcvznb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wntdlgiz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bhdxdbfi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iawdcpkx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yrcfvmok.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ijipidwq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rggtdeha.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yabpxtly.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ychdfvhl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2efbxhjuq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2emypuydk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mfnfeqii.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fyuknbtm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ksazhndk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ksyoewkd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cixmtoal.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xtkpdvhe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hjktdqrw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2czpaeaxo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fqybnmmg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2benpttwg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2akqnrkfd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dytzpndr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2igvwisyj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2irnshjmf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fqroumou.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2skjyfcuq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xbzrgtxv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qkffryzz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bmeyyeye.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ogsxwsft.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbtlsjgx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zdfjishc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ocolkgir.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nguzyapi.html


<!-- 参考信息 -->