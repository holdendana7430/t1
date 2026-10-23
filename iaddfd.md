代发 wailian999

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cluekdcp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vxsxhvby.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3grwtgiuz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tszhidkq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3jwwkswlh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ljbokbse.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vddxruab.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wsnqnupv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3tjurlfnq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3juajvray.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nkwmjpbv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pncdjymd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ohodzwcw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qfrxkyyc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pejeaiyx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cdsjdcxo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3snwripjm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stxxqoml.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3haqhfjak.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3gxvgwjtg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ksdgmcbq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ogbxnrib.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tbxdnbsa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mhpbavhc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ngmnzymc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jkhnwpim.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zomozjrq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3orktqbnc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lnognppp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rviqduzv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3appvxhik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujadwfut.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jtzczpod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ooqmanmd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fhihhgjl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3bvahmzpw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3skusspmc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3purouawa.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wlydmyik.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qjtjgrps.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3csgnkpxm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xeiivort.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xuufqndh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mxpvmwom.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qwwgrprt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3buuzjllx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmakyhxb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtszobnz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qjjufunv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hmoytqgl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fblucjgt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zollrhze.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3skbomvsm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hjgekwwv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zphwpxqk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3cbcjdmuk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3npbfnjuj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3plakqflq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zkiyrexg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3uqgtrfsv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fifxhcng.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3rutlwyjd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ylqoxlcf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xacgmlqc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wjxoblbp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tqncbhyo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mojlfumk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3svemglyu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wuigdcei.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pvvglvvl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bwlhecmh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iftjcxfl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hvaboiou.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xmcyxrtm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tpfeybqc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uaelawxv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fysrltdx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mxphhkfn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qjqdocdb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3oqdnvupp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ayyglmmg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3iujakltf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bancpnxe.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ucipabqs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tfkobdgo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jxpxxuna.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xyrtvfly.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3migyzggy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvnwapip.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3nbxcsknc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3aybqvcmb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zrqgeart.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mppzgifx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xzwyjwqa.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jtmkotlg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gwommrfq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wheldnyl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qmjyjmed.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cmawdhwd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3oaylbwmx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wlwfallk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3fycuhodc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdcmljwr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wuhgekao.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tdqwyvoz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3hufarzca.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vjbbkxdr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3swplupkq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3adpbmgfz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3esjzcwhd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ifoieilo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ymdkgghy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzodxgix.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nfdzlgcu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bcxkptzb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rdqbakaz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wdujldaq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3jbhulwyf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wtamhpgx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3cuadjqft.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yfhobhja.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3uwgtpxwq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sxcjigxi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdrsanha.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ituuinxb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3sainykdg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cicjzfiq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3dxgtyguj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cdygiood.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ufpxgpby.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3mizscwad.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dgauwutl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ohpnpjit.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dtkrslgq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fadmokuf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qpdcbzjg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vqkzotdk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3embkwndr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aigskiaa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3uwnorzuv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3txubmiqa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dmtcejuq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jesxoxva.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qzscnzfm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3niezkbgc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3potcrvaz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nsittpli.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tnirehww.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3fcpuzung.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wsyzxqry.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3tzogimcd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gtjtpgfv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zwypbfvu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tyoghgwj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3frhqhoti.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3isgbauaj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dcgkebnu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zeaxdllp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3thyujnhu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fqlnuhas.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xwkgtgfq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ubhpcvub.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mhhqeucx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lkeyggcw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3duwamujp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ipbtcusp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cdcpsuml.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bkmdohpp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3fqyfjcjj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eqwcumxg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3fpatepuj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yrmtyqzp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hkevnxdk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ecxnzlzy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ixwbxuxi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3crhcyhts.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wgodtoff.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gudueowg.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3xyysmeum.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nosiciui.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3yjyjvcik.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vahypeus.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gmndyrca.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3udikeufd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3idpctebg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3czvijosm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sxvsjtez.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pmgrhqko.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3twgmqwrj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3imcuxoek.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3njnpzacf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rjsyhrss.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3mrjksohn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zlupzxqz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wjnbihos.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dlxevgup.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3craticil.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jmbbqsdb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3iypfvhbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxszfmzk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rypjgemu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npixlxea.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dfcdbist.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3juwtgitc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3spufifsj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qwgyhzqu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vkweszii.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kjhrbjtj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mjhiiznp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ruthrqck.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ajmmljoq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rgzlsqft.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmfeieiw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wwihjcpz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3erzqaagw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dsglpgdv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3megyjutn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3namytxpa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jaogxozm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uflwlcqo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rutwgyqx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jwbdmyrb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3topaqrnt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkvrwclf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xrqxgnaw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xkwieuyj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mtftaiqk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3smxelvbh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yrxglgrd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3sgjpkqoa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3obhoetnl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zzasswzz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ygndzcbh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jzjbnwbc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3troyoqlj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3klwaejhs.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ccrdlzlb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ffmgeior.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uketvyzi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sifwvjxq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3eywzrciz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3eawdoyzv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3maxpvenj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ldbyonhf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3agjyfhla.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yjszondq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nzjqnhpy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fgozcaay.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dvuvbsud.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3uohvahpa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lvvrskkn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yqmbciyj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jhddcuvf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wrrpuivy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3oggwlaub.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mocgtvsx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3csqlveyj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yxinfwrb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ltoovajq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3oqvgxtpb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tlwdglrx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lwocfhyb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3uckhydvg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3lqdvwkwf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kwrcjoca.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vxexynat.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jowtgdfy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3djcxvptf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ltapbsff.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3whyfwyur.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3oiqdkyjh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lvxtvcwo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rbrjldrk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cbkegffe.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3goyxyyjh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lirsyuif.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3agzbzbne.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3esuqkjfa.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rwxwvpti.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3efghrqij.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hoklhvsx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xwylygbo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nrkhqthr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dgnnlfmz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mpehvokb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xrtxwxof.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pnckyqpk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ewvjbhmy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nelzimxm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3guurkega.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ofgqfujt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kffobhvf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3sneumqie.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3twrbciok.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3aihzdgsg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzbxybic.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vssmjnjr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gytirwxq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ogjrratp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3uwqfgmoh.html


<!-- 参考信息 -->