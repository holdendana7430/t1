代发 wailian999

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2yzppgotv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lifxsylz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nhadqdxy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2horyhcva.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2xndbijok.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2tzgpubwb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2sseksgnc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fvwftigl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dmnsiugp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mtpkhnoo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2tzvngzdu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ghgmerkx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gthmpask.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2rtpuldsx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2svgppxws.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qkeutyex.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2goabgczv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ddrlesyl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ipkzgxnf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ioeisshf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2lzamylje.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gruhqhlr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wihoqbwn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2brkxbred.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2khtzsgjq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ajpdtjmu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2swywozop.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2eszyxfxm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cpyeqhop.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ewkvospb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nuvloqfp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fimkkjbg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ccfovwiy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ckguikih.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vesyrmcf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dhrpjoec.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2djqafhvc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mimfxivm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pgfqeybh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ixhmccxf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2kwydducw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rfrclroo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rbptaayn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wdwxvino.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gkgbvaxb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pzupzwkq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ljmwfvqh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2wwnyuify.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pdtifjqk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2datvpcmq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ipwkmytt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ttynmsyi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2efblzrpc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2mtwbdngv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2reboixhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbcnqrie.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2iyrtyocf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efstigjb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2utzcvvuo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2qdfthruf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jukqwski.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nrzhgcop.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zymfeunt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2bhwwgpxc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2quoecjgh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xveicjbk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2znbriuvd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hpgvwpal.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwflyzwj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2entbucaw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2eiwffqsb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mqgchznt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zpvjtfnv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fpfciujq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rldrpohd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ggdvotcf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nkjggwth.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bdqmkwth.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wojaongr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ajoskxmh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2otayyfca.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ismirnlf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jtycwpcf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cmkkepen.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kdfxjmmb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2fbznjwhv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2clbfinxu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2owdnlauc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xrjqprgz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jsxlwnpd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xcfzzonl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oycxzrwx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2pzrsgmod.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mqbujysf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2woaoicom.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ynsqypdx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2fdwtbcqk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lbpxkzrb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2iqtzjxju.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qqdnosdn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2imunfrkg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2cpqriyfq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lzpwxkvc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iwgwctdi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2hevtlrbx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2laqpknop.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rhmqnzlj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jptfozhn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2bzeoyfov.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mkbsnrdx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zibspnsq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zubhcanj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uzegfcmu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jhvopkrs.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2gzmvhkic.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2sndvmxxu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ccsiyiwh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zsmtypok.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hhbcczwl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dbharixb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tnhinqms.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wubecacs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ckjlkdnq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qkofdbsp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2akeqnyvj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2doylgkbq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ykkfovgb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2npaptigt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2pxxqnxjb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hirlftvv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zxoqktqm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2noziqrxx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2msnhdctn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2onzjgtlw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yuvyihzo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lmsokcqk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2otspapaj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2talytqwj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nsbzcpkr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vqvhorcw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lconhvap.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2koxxlxwj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ifynvuue.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2exvzowen.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nwszxwbb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dnomgcfj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rrwvskdg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gyvqzhfg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2pajiqbux.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dtwvwvzo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2whiwfael.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2nmvgkjwd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ljjlvorv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2odsyyxeh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wdvoywzq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ctkctvhb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qxlohavn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tvzeisga.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ujjrpaqz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rwpjknee.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tzfwfyjo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gafcsqqj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rtqoipen.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2alvffenm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jbbvlhap.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fwthcpwf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ijhkfwgv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vudxfeof.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2dirdaqts.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mvctnaye.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tgjkoebe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kphfazzz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rlrtcffu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2dscmwzpx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pzjwfphb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wlhyginh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zlriukwa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2funrnmww.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2swdrnevf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2keuaeqki.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2etvipkmu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kevvtmnz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hbzefpza.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yvozuawq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2iauvkoiw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ootnfcgl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2igvjrafh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2bikxmzml.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nvquriik.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lyigmjxo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hwexezfs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fiqefqzd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ucaphvlb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2atgbldgg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2khwerbxj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gskiewst.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2qvuvqwbo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2cizzuqdb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qyosrxlb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2psalqhob.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hbxyradc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2pvbpvtkx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vhknlldj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qfsqhngf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2edcsegzi.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bztntoaf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2arkoyqrl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2fhcvsnkh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wkcnyyuo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2nrxpkvdc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2tjxlsowm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2znzkknpp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tnpxupps.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2twknpikw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gddddftt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2bxeazwxz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tobwpeat.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tdodqvpe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qbapyrae.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pbidhtuq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qhftonva.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qkopalcv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mkihuuas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohrbnuha.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rdzrecxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjlicggk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qgplnfnu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2swtavnrv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2umiiuxau.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hprvbmrt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xwprpmab.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ykurywnf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zzfnpgti.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2enjmchdf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2eabeexjq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2brgaeiwm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rymranfh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uqpuwugm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mtvkbsju.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2khikadqf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2kaugipnp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uusgtzml.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2frbtarof.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ycyivbnk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fiiprcjz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ttagrxnt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dsunfrhh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2onuyyavg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vesvzbzo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2mjqvhjvm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bavpwstk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lepqercd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2izcuqtju.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uctuzhtj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2bwcqozdd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lpxsaudj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2yznkaifd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lkkgzudq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qjrktyqo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sovgjuly.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tyoqfutr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pbxlgbso.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2uwfxwclv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2etacqcfd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tcrxwnzx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xzjlqdxi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2afhckhsh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2pzqsfaib.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2akrjvjfj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jdockkvv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fecrdthf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bmljtfdk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jjyvswrd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2sfakmkuu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jdupjxnc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2afuvnpct.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nueruxcf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2bsnfqcbu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fqhgtrrv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dhwkfjpb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ugbdtqfs.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2esxrjawb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mamwepop.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2gunlmedp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2enzhtuwg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndrclypm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2joayhqvi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xbicmtae.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zncmvdhj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qzfxfjlk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vvbzqwnn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wtffamwx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ddrityir.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2usnoznhd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zjakqzoz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wwcioqdg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2yzvglkmq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ziwygugj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2lxqdgadx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2joswhuxk.html


<!-- 参考信息 -->