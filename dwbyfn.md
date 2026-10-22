代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bkjwkmrz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ctjgulkf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2piqvpqlq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ucmzjdjb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dqvthoqk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wfugavwp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2chnjxftm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hycosoik.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2npdzhlne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdoyiaqz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cpaizhdl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ovjnfcnc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2bfjnvsdv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qasyzoov.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xqmxzvln.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2esosipfu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mdcbmzbk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2rdeimmrq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jrzjnnpc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bimfoeox.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2regvfhow.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2oelcvdyd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uehopazs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2yefvxkhm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dwlcvzzr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2icjayyvh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sdirlgca.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dykhwxcp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2cdpdsksy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bslhrpxk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kcjtaotq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2zeomdxig.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qcwhcpis.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2spmwpsgs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2nuxqorif.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ajybiewx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gemvvbpk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2mrjlfqiq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2cunbxxjp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2eqdjpwaq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2iesfzsmx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ntbsukxa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wrawmdfv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2muuthbfg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bmrnafyt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qufiqzvk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rnomjtcp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2omdotxky.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2scdcsyus.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2oqyksecu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gggorzqk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fkznapda.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jockjfvk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vfcicqfv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2moxmchkf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pmsqlbdt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cudfrhri.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ooblyjjc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kyojgzti.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fiauackl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hvauandt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rhefmkoy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lhtiyrcs.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hxuuzeqe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cijthzaf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vymfrxyd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2gvwhzwlw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2njrcatnj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xbdixrdu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2drcyzorx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2limtfosx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mmykebnf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2iziwviks.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mauivbff.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zkcaasaj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tlznvkve.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwrpxjzt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dfcvpdvk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xltkphkb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xmaucxdq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hpptnyea.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2suwybqxt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lsiqzkha.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2sytjsisg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2odfcfqqw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xzzvqbqg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2lvgnwbut.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rpaibyar.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mjkwsuhk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2djmkjzoh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dwmuxlzs.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2kdqxrgqs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jmpykuwi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2nblmjwbw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tloexsqt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2dtyysezc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tneeifop.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2fqlebukh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jyhyvjds.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2abepumok.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2orbjwbii.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kqjaoudg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jwxnrczr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tuypkkkw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dzxbldby.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ezlscukl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nclsmzrk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2lsgfailz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fugedkvm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gmajocgn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cyhxfsqz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tyyshogx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ypoytxdm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2fiufndsy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mxnpmtch.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jjqzmuni.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2gariscjo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2rknoziee.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pzpgwmfi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2yfjeljth.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2jmpscbcx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jsdeodme.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rmzuhoil.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yfrihjbh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2avhcgnme.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mqznhyju.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ifljlsvk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mhejrguc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2owghauyd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2rtwnohwk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cjhchxus.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ptnneail.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vxvhstty.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jhqfzfta.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2yzagixdo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kfqsbemg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rtbqisec.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2mrnikndm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ireugvqv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wfbgwkny.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xzzejeng.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yyclabkg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fllynfwj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dqgtgduk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lagyrlcu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vqgbtwwc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fvnqkfzr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2giwbjhde.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2fqkufznt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dlprfxxs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jqgjrrbg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ybcywrel.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lvqawbls.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fnvkdsxn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ncqxeixy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kfvcfylm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qtlpfofp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2volglpwl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xeyilget.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nowqbuzl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2oamxdgew.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dmtxvrrr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jfgdvmmf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cbudwfdp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tawmztpj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2efpurprc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ozskqubj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2kpjqbzix.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2hvrtfybr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rpkamgaj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2oonjzzjh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dgeqwgfb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qvkfwcik.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lhnmjfdq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tlrqpnzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylygirlb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qweocloz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtxuicyo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lqaiauih.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xbgwhwza.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2qrbcwvxc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dzsuooej.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2sqpdyprl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jtziookx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xoetvvgj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2rjgbgkkb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ndokmjuc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qujnjado.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2fbjckzpn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tcizcdci.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cxjkukwd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rcksmlhn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2isksrbrd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ifzmswwt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ebfcvhvo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ykhbagxr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pghtedbd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lxwjyqln.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hxpjkkmh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gunoyrxb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xtjmkbqg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2djvnfzoz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2plbkzpqy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bsjflrsg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2apbpnhcs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2uhmhrnpc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rjbqiace.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yivarmas.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dbunqdwu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bfrwfdob.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2eeuxluhr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jldupsmi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xpvlghxe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yljxgljb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ievlscng.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2apdjqyth.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2cfofehyg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jvdbjhiq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pgfiarzr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bmofpnkz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lmwirslb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2hvhbklfs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2jseijgfp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2syunghta.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hlybckzc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lclpkvuw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fezysagj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ugsbmmnv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2utnhamja.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fpmxpewb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2cfeisnsi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kuuflbsu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wnpkyzkr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2kaatduiy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rhoztevv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2zkpywatg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ipgyypjh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lvlfgbdn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2fvmdsuei.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2nwyueovw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uygosnck.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cqhytxtd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xsadrmwl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2towfayzc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jcrisuol.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dggpmqlj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rvsucmkj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rqeasojp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2spddpazi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2kstuughl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zrlxskcg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ujcyjwqb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2kraxvwct.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jygicmbn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tthzgfin.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fxzfvpon.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2rbgdzdzd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2etkrrdim.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2oimafrue.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mclniufs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jtaqvcxy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qdcefhbq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rtmkcege.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2nojgslow.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dmjbhuqm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fwvyvjxa.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2aokhwccl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gkdfautw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qvrcelwg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hzkrqkbx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2buktvtdn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbheguwp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wujbbfnz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zdrylcvo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rltdfyjp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2larnjpbm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uyxwiquy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnnnhjnf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qqcuajfc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2kmdxdjdh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2usglfhck.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yabbnuqd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2kkagjzct.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bxtihixm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ypzzdbes.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mbowgyqc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zboiklgo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2srjnthvg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pecdxkht.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2aamixxts.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hmnagqzg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vfwmghbb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iviueeap.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2llmqtelo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ufauxdax.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qzdunfsw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkodaoes.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2psaphppb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ymklmjoe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nbsyjggj.html


<!-- 参考信息 -->