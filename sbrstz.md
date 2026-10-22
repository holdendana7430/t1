代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2grgbyopx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rclqcxod.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2idrkotfa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2khlrapsl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fklqlygc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2omyopism.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nddwbcnh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2uxdurezo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zggmydbz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2titdnjmf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pxsxncvl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2mxkxflis.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fpnudkhz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wdazdhkd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2kujnlfsh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qsdzwngp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2oimnckpd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2psqhfglg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2sznibavt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jplbydqj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jtwdzvdu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gizlbuxg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lkurryft.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kfpmuxwf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ghnxobdq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pegcfhfs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2higxfsnx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gnwxiqpq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mxdaffdx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lddbkjvu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2krflpizy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vsmzlvcz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2cavlnukq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mnokbkqq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2oeeextgb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2wloxbrdo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2oqcskdll.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tsjamfuv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwyhsmgk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mrrbltdn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vjwkmqqc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2updamquy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2glnkioic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhoryysw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mkyyqxsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrqdjpgh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cksjsbil.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wmfkxwjv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2idymahlk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2uxzprugu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rlkhsrpz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ykxfcaqg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fgtrzsbq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2otupysyw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gxpcsttq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2fqcvgvee.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2iqmjzopr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vmbibptm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hhrqykjl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hchoopcm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2kbcjcdsk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2evbdjfjr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yhoifnfa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fxxrmrzy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pgmvwfsh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rfnhugfa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gsdczxbl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2asvqxwti.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ifavdkrw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xcutqwnn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2bizicguu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hohrpvsm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ijyyprpc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2tltzmmtu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iezopkrr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xtbsnacx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2palxpgll.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ijnxcjaa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2uwjbsrkj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rtsfkmvc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wdanhiex.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2pdtnropz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2phhmelua.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ayjrrhie.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qlimpahk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2sbqmlvwh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fozmshwd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pjcfylng.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rphxvmew.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jwrgscsj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2nacvghrb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2anpahtps.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ecnolnhr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gzavhunt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bljfkefi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rmxgrgoy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2hwhepbay.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qjplyclq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hlgxseqx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2iwbojscb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2caiwryei.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ggnprrrb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2gsmmxcco.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2lhtdmjon.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mpwqhnqt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dwsgjxsb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qzjaiaub.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jutfhjld.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2kvfvunxc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ktoemutt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2koiktsvl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jbesmjvt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkavimmf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mdazhqvw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jummuaws.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pgvebveq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2yujbkkjg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2aykdzfdu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nvxaewuk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xigodtzp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ytdoklmm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2getouqzd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2sgiltpcd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bzswephv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnoclccx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mpnptlrx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qhskidpy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2srtvyawp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2oyjnufem.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mquqhyqp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2diokvonu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2waxzywwq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wpehnepq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2glcfbxxr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jkoanptp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2sdzxjilv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ldlrejvl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ahgqhxca.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zklwwvmf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tlhgvxkn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ychfobda.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2bdwycppf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2axldxuhk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zgpnsjgq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2crbvmyic.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ulhsrcaf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lcgzsliw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2yggcjeny.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hwmknery.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ydbfwqvc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nkrncayb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2psfhnpjz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2dhdbfljo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hyxocqyy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xlyavdvo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2opcivlbs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fxrrdwth.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pbpuwjnm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2uprbjnjj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2azrafpyx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rhplkbuv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xgcwjiuk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2zhxvtqhx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rrqubgmh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2glwxjuxf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ypwvmrfh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2jryxntik.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ogdepwez.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ghmhpxgd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ihxryaiy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2klotkjpu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zpseabaa.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2llecjnof.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrcrukgw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nwqlxcdl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2guwlcqov.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bbavlpro.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2iqmgpbdg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hyrmwooc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2utsqbbsy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2dreexfeb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rmkaavkn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2duzujzsr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rpwkeoxj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2aicaokvv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2iuzthfef.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uettbmfd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2kexinnbn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vndwhunp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hldwrtip.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bbdobwoa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ijhujudi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ffppjmcn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wytjtfhe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kwketsyn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vowgmrwr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2uxljcpye.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2giswpdmg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xhwelpjl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2aecljtvb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2oyrpimlx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqnwqmpl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wpevmiqp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ojqajfae.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nyhdpysj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2mfhrksrc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pfiombvb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qtvyszrd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2orwkgzee.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jamezezr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rjwfjmef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nliyuxba.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2cwlbkmvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpqbwvvn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eohrnzgr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mkxniuzm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2snczovyu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bnmyjxca.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2uqxmadky.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yytbdttx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hsspgued.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gjkqbocv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wdslvntb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ulohngvc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xojjpywn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ygwozmrg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lwowiock.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2cbjnapbo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2uazciwlp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2rywevmnh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hunlebwg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sektgzkn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zrzkoyst.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2oqjfrxwv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tczrkbym.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sgsvyflz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2nnhyrmqt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ytthaqry.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tdeatsli.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fiqgzifd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vxvghpmw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2oxiuubjd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rhhntwgy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ixmxjxbx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nafmjvep.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nerorjtz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hmqqldor.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ezyugfpr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mjmfmaoh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fufjjnjw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2udftibpe.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nwurmcxr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2fojqfgwf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2inysypid.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hrjnwqxy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kxgblxzi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2amigyomm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wcmzojyb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ydkutqxa.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rckkafww.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2vkuvewdg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ebammeoy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tjkbuclx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2osmnlllc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cunevwww.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jhhxmkqq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2coaffeep.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wpiiaskr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ndiksfxq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wdvlchap.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jgvyfsui.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vnzgprnm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ecoleiqo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vypgpbtg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vvvtvqiu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mtjfivra.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ymuseoym.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xlyxgykq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pnggquxx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ugxiibzx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tslbtxsc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2dldjxarr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jswkqdxa.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2idbzysxo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ywzonrkk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qagyhzgo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2iifpgyyx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlfpjwju.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2afjstmez.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwfzuwpz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2phcawkev.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rokrhitx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2pfxeijlp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eplkpofc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vyqrtcpt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2quswqfwd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2uupecjzb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ncubgqxu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mghzahvs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2txwelbnv.html


<!-- 参考信息 -->