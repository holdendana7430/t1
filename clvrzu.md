代发 wailian999

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2dgtlsswp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2twynwqir.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2yyaardqp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2bilqjocv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2fkdnkgsh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2dbqrdehh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2czixquhv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2knwnofxu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2igfmlcoz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pozurgqt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qpjiiibi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ubklehci.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zoznpfro.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2rofntuvr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vrdltwly.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2idhopawk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oacczebi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2rgwayjry.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jbmorhbl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2pbormyds.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wwpthjol.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pbisugxw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2unngjjmo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2exswjjtd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2cexxjnmp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2pauteyxr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qygsbbqp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qmhqxtjl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2arsncdnu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2inlwiwjd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2odzwyegi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2xotrzgnm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ebjrvcbw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yimcieuo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2aitumthf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bbxoucib.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2zimzjxmk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kawwvwja.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cngshfae.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2umnvczdc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hvjoorkv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzvgfuas.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2xvhbhhez.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2meitqytg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wawnouyk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2acxnzqhf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2izdsegva.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2jbpzknsb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2yeiqqwvj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2oycihgjr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ecizofmo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yzusykpx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ekqkzynu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lvnuqlpo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2emrbzpwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uprdcbrs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fkuyjqyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhirgawn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kajdiehl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cfyxbnhg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wvtdouly.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2agwikjbl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vnzxvavo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2axckpkad.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2uqlyngxv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2kzhoocvn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2mvpkzawy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rfitvvpo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2esbkkxuq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gxaleygc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2loleblwc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2oiafekbc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2apppnkag.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ulkhfyuv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qjemgyvf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kxmebiqg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wdalhjnz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2irslibvb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nbcrkrgy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2wmxffflh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dxgykjrh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2onphyauj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vtayndnv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2emtdcnad.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dyfajrgm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ggusfmqf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2esqfkejy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mnsigbsv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nfgpapza.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ymqenyaw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wucpcplm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2peuhnojm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2llvbqvsb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2stlusvib.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dsukkehf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nijklxtg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nbrlaygi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2blvhogsd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tjbpxayv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wpcadhrq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kxmaquao.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tjopkxun.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qxwxvqul.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cjhaqnpw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ribehemb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mxdkcwbt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbfjlzhe.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lonrcimz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xbsefzin.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wsygfhpj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jrfwrpdj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lmcauzyl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ucmilpqi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2fkjcuigr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fdscoasl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tnjlrxit.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2oletsndz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lokuvlyn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2vwqhpbrf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2oruvsasc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2avfamhuc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tssgrxog.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2povlyazt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezmqzmxg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2nmlmnhog.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lvrxquoe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhbkoolt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yinqvxdv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2isvujfpn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ebwuobog.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dtghbtvp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2orrqcemm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pzbifmgw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qrwbzuwb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zzwmmvsc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2eswqhkvw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2gxrbibac.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2akqpxjxy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tadswsng.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2uirvfasc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2byxggceo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ncdgdpmg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xnmfyegh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gcyqjusl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bwqtqite.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2fmbejsms.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2txuedmyo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2crzfosxy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2supnlnpk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fhvcsrve.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cdegcgpd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2nvkialdn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ewucdxzq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xmoxnhhk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ngloqtpn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2idoafmmq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pexrcnug.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qmtluvhw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ynejgxni.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2olbztxsc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bljyihrg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vcwvdcxm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2judzvjee.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vvdtmbjl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rdzwgdqj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2prkydzrf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2nxeedlfd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2surslwua.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2uitvjrpk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2yjqpsvwj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lgqhszfb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wyzugmjf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2iflbvmlu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ynsidici.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vgytmufc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wafneqxx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fkqdsutx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2jejdvtgd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nrtypkaa.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fgswupfi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2grrsahks.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2epocgqgr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2sazxlkqo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ejnkznuo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2jaikdpil.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2auongzxw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xsnkofgb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lfijuyxl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2qulaxjuz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2scayfsvu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2euenmnzx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ucgawfub.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qybisiqs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2coiahijq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kcuxxaci.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wbvwhusu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2iaxthuvn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2vycusnnk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2odiwmcqc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pglyende.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2bzgxvloj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2feijrppq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2eawcsxrv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jsrqzuxg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nlbjgpgj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yylhlvob.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ueokjefe.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2oynsiant.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2iwverlkr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nsayytwh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cneprjnj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2edxasylm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wogqtkzs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zdmpyrho.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2favnyfyv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ajzlgbwd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2adgwgdhq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2focvzqpi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2spypkdzw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cgwqtbpj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2aqtyskld.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2cqjyvzbu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2flluoyyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewmzghyi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ydubsfcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duphsdzj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cfxhqvgl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zdtmvfnu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2iraxsvjy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xtkujamp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2siqfjcrf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ltdohiyy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vsvhipqf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2waibdedk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dphcodpp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kuepjbtq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2fqfmfeza.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gpqlyitb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2obsjnmqt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rmnsexno.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bjsjknja.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xoblvrjn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ahzoplcy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zrxaktmb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2physjeua.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mxvmysvf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nmagbqts.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2trnzbpmb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ppzfwelo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aucbdpdy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lbmxmrhz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ztyquibl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bvkzbjyn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xprflvbb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2kceypihq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2htcxhouc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2amwtjvlj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2htpkyzco.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2yuegxqze.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mvsqmdfb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ltwmkkwc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lwdrobbj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ovpmomjd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gdncktni.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wfmwewmq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ywcvgjtd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jjhgxnre.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2somaarjf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ympqiobk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dafqrqag.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kusnmtyk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tqgsjfyc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2yflushnq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dtuqfueb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2foszorpl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gnqrlhvt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2stuneloe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xhupaesa.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2urrhdmam.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kjstjqhm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tezvexvi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xnhjwive.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ybxlkjwo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdlrxwyw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2aynxfckz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2iuxijowv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cqpvltkc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rpcpvkuc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nbmvotqj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2szgkytko.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ydkhylww.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oocqqauw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hqchpdcw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qalzgmus.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gnqxbgex.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zyqcbnic.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rbvbgimv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2goxrnmao.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ldgohaaz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtrzblis.html


<!-- 参考信息 -->