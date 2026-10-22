代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2btcvnzub.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2baonitay.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bnxrsolc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2juwrcaca.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2iiqwqbyc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ykfkidpn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mpayjzgn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2sisunyoq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gkmjbevi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vpcsyhys.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wrxxpsep.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tygeaaxu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2lubwrsij.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rqljqhmt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lqeaowhr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nqmzneyj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftwjavor.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozvfarsw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vddxhvfe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iubrfvdg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gisqklqi.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lrtkpwdj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2soczcmwz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dwxjtawi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qohxbcsu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gjgbmksh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tbhxbjmq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xbxzizjn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rvfobqal.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ebjfpyor.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2flzlebsn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bsaapenw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2icuwhvwm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vatrrskn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2juuydtzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrmsmblj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kfukyizr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjoqimqz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zbhnsold.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jvjcdzqu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ngarflmi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xsyboodz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wnrwnkkx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hsairnwc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2iwshhdjf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nzukgaua.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zbqubcsu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hfcpofxo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ufnzrgbz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tjhqelcb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2eltdkuyp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pilwzxde.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lsngmagv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2yjizspgs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qgzwrjkc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xysrncqs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qabfwhjn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2trfxkuec.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xmlrbltj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bizucwyr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2urzahprc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hlhalxrz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ygfibvgh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dhewcisr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2pdjzlopr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ndvxtsuv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2udxtfnwn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rbsvadyy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2odqxcytz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dmwraanp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lxnpgwde.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2myxmhzdm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2tptkfjaq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rakndime.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yvxygztx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ruglzykf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mfdginlb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2teggpnpo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xtigpnfs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tpmapley.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mnvuagtq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tccteydb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xnukrdvm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cqywrsrk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ujmjuckz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rbsjpknl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xksalswq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tzqgexbf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vrlqrjsy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2phczlbpi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2hgeokwjq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2uzoxkflt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wmrejxlz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ezslvycw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dpdzgugj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sppgvsem.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pnuekcoz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2dafobilg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yahcvnpj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ecvxbqvc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2csvsxcqy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vfiquxjd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rofgauwd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kdtgnadd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ngoglnrs.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2eyvgxdpw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnfamfrt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2keretlyi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2efrumiou.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mpjqxuup.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rrqrlrye.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2sbufbtvj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hofiqryg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ukpypbyi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2cvucjuyj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xipkgiji.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2rxnkczzx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2gzfsclia.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bslwdydj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zzynhvbc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2agtdkcox.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2llsmrqem.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2artzotdi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gqhosvkw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wnoyshig.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xxjxdygs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xzsjcwhf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2dmhtxrmr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2yhgpxwds.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mqydicdn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hfrqptkj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hgqzshtw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2giiigaqt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2laphwgoe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zyzkbyxc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hiqqdiir.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hgmbfcob.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uyovwuib.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uksixyhf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2oguvygvr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ccjzedhg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qjjpyitd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2egboxwml.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ohvaiayr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2koytkqsp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cgqkxofp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hdzyvrit.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wqeygwdo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2iygycwri.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2vaujwvfy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bshamhdg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2fjxcwssp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ldhncdwi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iinfulme.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hsnoezrq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2czdmwhsm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tnixuhsd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ileahbxd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cdpyfaqv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mmaojqvc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2cdiswayr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xhfucfbg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2patokrto.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2erwdtdvc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qiesendd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2covrgbav.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qzmrxqli.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2olyoqbvs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rglxznxh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pyndoxem.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ontdbbow.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fjqmoylj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ylydoxgl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2sjrckaxc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wmlgrvtm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2eqijrudt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kfpdhuxe.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ztmobdyf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iggiiexa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ufdryrjj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2gwpdndwy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2peqkaiwe.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2girbonaj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lvhxxlkw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mjxkcduj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kikzfucu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qlvhwbbn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2agzzwmvf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2sttnitoi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wftttpbs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ichwngky.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kmoloxys.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2esocyvax.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2hivfshdj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2riqsgewt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ggtlfnbi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2sqivjues.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wqalzztr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cynkufpx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jdodcmto.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xjufwcfc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hyqcsrnd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wwsayebz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtlknlpq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zxxdirbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwenrknt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jdiuengx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fjmxyvbu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rqqowpbe.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vucuyncp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qohropxs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kvrswtja.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zhtpraxz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hqgtaszk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hmpydskl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mfwyvrvo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mecspfth.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tnhmxthr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ylhdstix.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hbjpntla.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2plssdoeb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lgvsheii.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fnqmbylz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kbdlkpwk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ydgltudq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zadkftkb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2uxrftlkc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2quepivhe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2enamrlvt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fadnsxqd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yznheviz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lstuoipk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2llwcakti.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pbhvtili.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2tillemwk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fbptjogb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2yfzzxcno.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yblskbdx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cnvhhlci.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rauwbtxa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2sdswxkkt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ldyrxgzv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ncgnbnie.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fqakkevb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lyevvasv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2sdyprawc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wtamgkww.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2msoxnuvg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oeucihof.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2yzxyvcyt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2qrjgpufx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2siholuzh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2prizqbqc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2wdqtrppl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2iqyufgkb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uncwypkc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qpqvoelu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uwxcmdss.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ltsbsncp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2olktathd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mwceydrr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2eixmterh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hrtjfush.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ndejdadb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rwptdfyg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2uthesnuq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jmhrhfxo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qqvycmci.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2otbywwim.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2crnkwocy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2eilqajjx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qnymfnhi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wunozhvx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2nfrlqfnk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dtkbztnd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2gdtrufer.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2noaxjtes.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yogzoinb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2uedptrgz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2whfpbdgu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ssacqvys.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2egxfciyv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jeksgmup.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cvanouka.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tbhecwzp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yvltrwny.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kazmpbhc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vrjprsru.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jdzfrncf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wguygedt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2eglbkliv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ybjwnfoe.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2syeuhkdy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gnlwzipz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gzefblmk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2whttfwnp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gwmplfun.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wpdkmyxb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ppwozzvc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qgmjrplh.html


<!-- 参考信息 -->