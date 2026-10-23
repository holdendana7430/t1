代发 wailian999

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zstswzjz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qrohgmge.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rynjvozc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yvntqtyp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hizxnqam.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dosqzhws.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dfvjncxv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fyhafdgo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3webimfla.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mxzjxrck.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bsqkrbcd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tqypkspu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ahxccuaj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3gagduwfw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ephbbcjs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zmdiibnz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hvdvojfi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xeekqpbh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nmofnwvt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yaodddyk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3fmtohmkb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3enynjxil.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cjyogcvc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mjpsblat.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fokstamg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wlxttmkg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ckumpemo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3wvyvbiou.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3pgxnqwzr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rordzpqp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kmvucxjh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ktlcyihn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zsdtrjmv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3gpojyblb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iiiyfkls.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xzsuoxsy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hzlujwlj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ckahxkeg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zqrrkcoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgcnvams.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ggpshxgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3inggpoxr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3clkfgfhd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pezbryqz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vcdkhnku.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kztxqesy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wmsamyjq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3amprfdqc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ynynwvze.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wxoptesj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zdpcbxep.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3intlvcxk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3bkrghpkb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3erxnlylt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xmysnyqu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3otdohimi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sitdsjeb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dsqojelh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3udvvaghb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vmvjavbp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tpfxewzp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3vryepqhj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rtgsnugk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hxvsfkyo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3dwfypdkn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ozuyxgdi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nivbacjq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nvdcpsfo.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ivvnkvbo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfwpmoyj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eqedljhi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3onpfjhao.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fpohvyrw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zqkxolqh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zxhmzamd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kznfehux.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aisrhzgp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3elvmcfnh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jiggnlcq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3cyyjikyx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xkqqedis.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xdalamvg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gvlsaabh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nibeqvan.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rhinztee.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qahhgcmp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qrggjxkn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hiyejgra.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3qytfeasj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jfzniteh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qtklmjvq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bgbgbrqh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3zzbqzrfw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yphhaebb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hjufyldu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zsdksvog.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ipihwmiq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3enersrvs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3uhaakqfn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tlqftnpq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wvtcliqz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dxbyegcl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ajxdifap.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3aiyicsxc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bgzzqtqe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3imfzztla.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yccyjicu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ukinfhwj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmxqmqmw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3npyvpiip.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysoaotxq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3uengahtd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3enpxjkha.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3oqbilijy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3erlmgzcs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3isszmbty.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nroldwrb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zkosbmwq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3thfjnekm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lavqedcp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tokjprlw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wjdawsai.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zaasrdky.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lfmeoyoy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gbsqbsfp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3hhmdnooj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3oucvbedo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ykjxpkxf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hqvmxpem.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wqldfotr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3etksasxe.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3sqdynwkt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mknfojfm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tyzbsjil.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dwbcgdgx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3gbetqjrg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cipqpwyx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3xksqbyll.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3hnidmlik.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3gcgpjbla.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wpixiitp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fyrhdxbx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sfjaikxm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lktgqces.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tspsvfny.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3apuptcpz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pbdtnsof.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fulomibm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3legsqnnw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3alveedav.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3isdyknrj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vlomthwf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3iauyrxnf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3delydoyn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3snwbdvpv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bankaphy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ogtahsbr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3tmtiufho.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3okwolzsb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nqmcwwwe.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ezrchzaa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvwvyhpo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3chhghlus.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3blhjwepk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rvosjtje.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nhlhflcd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ztwsumhb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lgweythc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tlngwgvf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljjjmcid.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3cezkihiq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mmtzmuqf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mzsxxamx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ebjtnntc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cacgxesv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3cgormpte.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vspcnbxd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qeiwcfln.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3llpsrafd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3bbenqlgy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hwagqevy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nnybkpvb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wzxbfpyg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lduhnwdd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yqczxbud.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3onaqhulc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mlalqojm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3izncebyk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3kxcxjjhd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pwnujnhy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fubctuqm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fvawdrll.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3noevwsgl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3skelealh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ekwoootk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hcmwyukf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nttndhpe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kweazbom.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jiidlvif.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3uxklnsak.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vobtzdmz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jplnnwga.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3rrblyfum.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vvzrtkoq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uhdtgvkc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vhsnrefy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dsahhgem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etoqxxkw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3xoeppkxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojosqkdt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3evogtopj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3stjebjai.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofugiioi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vizdawgu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hpwvwnxx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3asrctsyg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vqtbfnow.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3igmaenzx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3iwtvegcj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tklwupjq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ddkmnazh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eiphvqem.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xgellhwx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xfzjmtae.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mlfwqojq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jtmmgkxa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3zhxnuwml.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3eselmapi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gkpbfqiy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lihvdkft.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vdqvcgbr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqbvltny.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jotfgmrn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hyrmfozv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3deiglqxq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ysflzxey.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zwwvdteb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3jplklezw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3yhacyrhb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ctqlrfuu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3zkczrsmn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vpotdvqc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bchaddyu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3pzgvjezz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vufdkbrt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kdylekle.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3simbrese.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3muqpvcqi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nksrsjon.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ljtkxppj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fkzoinpu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rfuzciga.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dlhpvrbv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zphxiqnz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tjuvjuvl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bxjkgoop.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3leswhqny.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3aajapwaf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wdxrzbqj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3woeevkbu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3felowduc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qqoffmkw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3htlyulbq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3obcfyaux.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qkejijqx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3sdijqmtz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3izugjzvk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wjarpkzj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cnpjocjk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mvelkydk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3itzbajij.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hquohzem.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3iayxethn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wvlcqdbr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hfwxtzxv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rdnogenv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wwxerkcz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3guqxzaad.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ldcphyhx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dvumrszv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nponzlyy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3sbqibzwb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fheudinn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ljynwuor.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3shvhekbp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qddlkdpv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xggidaib.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fujuqtdr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3njpijbyv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gvhhymai.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qezxtvpn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3calmmgpx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ywbbkhax.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3pcigtgcs.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qlboomjg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ydtjpudb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jkcdkpby.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pppguyou.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wwsqjpgm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kncxsfzx.html


<!-- 参考信息 -->