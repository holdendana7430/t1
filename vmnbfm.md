代发 wailian999

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vnlkfewf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rikgcmhr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lwobbgdd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2maliccsf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xfzxrcrq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tigtraca.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2culqmhtm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fytaktqe.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2gcwckfcp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dqbmvvig.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2iugsfmsa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2olpavhqi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bumukdif.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cjjedrza.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xdwjkycc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wsbxflnv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ynswzbxa.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hjyydipw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xwkzqfvq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ooiitmih.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xvrcqktq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ksgmxpsd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2aghyiqqu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dxxliggc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fkcjggrk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xxtpnwof.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2emzzaxhc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2swmiumsu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sgajvlxp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pifpnrkz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vgbxzlfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvbalvqf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2pdravwrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnvfkhxh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vpgmytmn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2riksvzfj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2asgirgcz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2fpwivkac.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2hnzikgzz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2cylhhnao.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cytgcxfq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xporwhjs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wrdwxvdm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2altmftdz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2iaowqzjd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2siyiiohm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ifzlphgz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dfenbvhx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wiwodibc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ikucbndc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dvwxqzif.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dnpvrunv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dzxgjbrj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ajlykoum.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2scvuyuai.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vypigqew.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bektyewu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jujyswxn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kfrjqejo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2inrupuzc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2uznmvzca.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pejferpt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2asgeighn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2liiqopzz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rmljatsi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lxypaimd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tmtguxpg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gebiodod.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hsdrtgcm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lfhbftxy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gbfdunor.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dxqgddio.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wgypwdzx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2hgvzvsnp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2butbpehj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rrjznwvi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2vosjfkny.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2xnfljleo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hyyfkwoh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mgtzbgab.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2amprmoqe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2noefkegf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2muuiqqeg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mofcxdiz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2irymobzj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bpgbytks.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tomdnoss.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hsazhemm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qqsmcbeg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jcjwxwvk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sibctvem.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2cbzukhtx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2repldtov.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hlnkmjne.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2prihmvvd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ugvsnbkg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ordstoow.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zydhfiga.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ikhdympk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gpbtkiyi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpghqbce.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kzhfpphz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxbjgfds.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wpxvtfhl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zmrarphj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hwimcpii.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dduzgxzn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sfrqnlso.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dyztmyhk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2tghtywmu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qtmpewtw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tgvhdjom.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2avtdhhgb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uqofzkly.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wrxdgrze.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pwpodcsz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wwyrzeva.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dsnpqbyw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ysocwatu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2beznmvrm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qayroxgd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pfhhccvx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vvatkmlv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ngdqnxyu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mrkajnxr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2cqdqrzvx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2agdaljpc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2akhcychh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rienppaa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2uyxvjbjz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2cejjdked.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cfbcuted.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zxfpyghr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bcolktaj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dhsjivgi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ripcilec.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lcqixtvh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2xdiulkco.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gftshhfh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2etktxwcs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kxntkdql.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2utyqrtlz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zrgmkkzs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rdadkrvx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ahmwewzq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2whmzuvel.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2enigoita.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2vojuzkha.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tfvppyqx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rfoibbnz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2dfpzievh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2cvqezvee.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2gzwnlhxl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyppmtdd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2emhlxaex.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ftrbrebk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hgeggecz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2madwlqqc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vbydutvh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ddnhnwxt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vvgzmlui.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2elwhcusg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zudchtls.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2psexeaoq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2tnmtxved.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mqbsbkvk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hjsinxgk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zzqkhyfo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2iiwxbtrm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2erloyovp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2juehigpn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xlkdnoly.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2etpuqjag.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2coaxrpfc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pwyyoyft.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jiglcvbk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2phdjrwaz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lmitvoug.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2uwljmpsi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pqhhlaho.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2pkwsfskc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2sfdjnmsb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2plymjlbu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pkfdakzo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wuioeujr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ybvvuuzk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nfujqqcv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bwvzmdjb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xrrefetn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xejnhiub.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ndanzuxt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ttdznump.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ymxakaid.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ebxhpaal.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tpgkgixr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kryjevck.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2alyipabh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2kbovpcxl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xmsfunzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtzupiuc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dbljgbel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzfpkord.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tiocsbyo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2yfgsijjz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnomyyjb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gvkdvvgq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2tjqiykae.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2njudbmap.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2eczzcowl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bhddslau.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rzcxbwzm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vnokaumh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbpxbmge.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qdvklyxj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lsdomamv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2unxrbzbq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2libkywyp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2oodmonff.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gbclduhp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tduxjymt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ozeewqmj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2sqzciuai.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2axxgqllp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xfpllzgy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2glaatmpe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2shsoddli.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dcptlmgl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qrlerdui.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gpuawmfi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hrnaropv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gymbexdc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fzikcjxw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cajxhyco.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2nbfqamcp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ytauaqmi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2siphofws.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qjcfhlcp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tqakjoeo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cditpejg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hiksurxl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xcwguusm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yebjzkrq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zedgxdvw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bfukjwmx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rkraaylu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2edvggrsd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lbfawjeq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yjrjmddd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wiavadxy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ntrzjfzd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2huplkmqo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2nwxqmaeg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2rokphsno.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hftcapwx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2agemnxdw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bwdugkmr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kxewyoxa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cbcavcem.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nozhvsoy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dfqaqaqk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qojazqwt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywxeiyys.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lxirqusu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2naaqxtcr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2asmfjrgl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wnmrmvst.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vqbtmvez.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xnkvuufu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nnnjaxqd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgykvjri.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zpuosmth.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2tsadmasu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2raksbies.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rkqqgtfx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ainnnpho.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuxnqdjz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vkrxvkav.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rbmfixsc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hzgxztma.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wkphgtqk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jhhpifpg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tfdfouil.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gxpkedro.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kbxbakbd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kqqlungh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rmkqaosl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wtszkgit.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gpncuwis.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2umtkwqty.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2dffmwqff.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2lqeyfiar.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fzztvnme.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vgzacqzc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xhksttzd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fleqqcii.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2glcskcfm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hqpasobe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2sagifoqt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2bqygpngj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmphfvpx.html


<!-- 参考信息 -->