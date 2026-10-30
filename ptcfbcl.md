代发 wailian999

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gemivzngx.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gvlrhjlvu.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gwytznuwf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxucbhngn.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gaowwcghw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvnzrkjn.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsamokeg.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgisjtdu.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gereecoge.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevshfzih.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhkzfinc.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gxxosuvmu.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gphnznhtm.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gkzlmwvaj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/giipspdgg.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzjrcidj.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grnnyuopo.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gkjbwqsot.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzzwxesx.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/ghweqsnjt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gpgbylxlt.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjgqjdtz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfaiduybf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gbuohpqwt.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gcmxraydm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmqgcphb.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/ghwtigrsq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gztakkkgr.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gtltzlego.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gmcyjtihx.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gulhwjhrv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gbowgczqj.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyjccmon.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpduxgawb.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghkskcwdk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpproxlr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gseczhmad.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grzcorwzk.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpornmjge.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gumnugjom.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrvzpnwg.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuuhnqqn.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyfwmjva.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/glaqmsqcu.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gshigxmbz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbtcuemz.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gevixhplm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/ggdwvrsbn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gayuillgd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gzlpcjskm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxosbbflb.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnpzunlm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gsagzrlht.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gbitpmfuf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdiwqbhp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gguivfrjq.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnlbxgtj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbsfbxlpk.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gngyxpybl.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/grnvvobve.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzspnlyt.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxggvezxb.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gqaddbfmy.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/goldyjrxm.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/grdmzdemu.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gntzattju.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtcicdjj.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpuydkbi.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/glmscbwme.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gifluxowt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisxjbpkc.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkcotpfn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlyqsvyl.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/glpdtbtef.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/goyfaekgh.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblzbugos.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gochepajn.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ghgoxokwq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/goyvmhqol.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gyzrsntox.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gehoiwwco.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfedgmxbw.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjhtxwlj.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdfipnvx.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusuzjzwy.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwykeitac.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstulvrzh.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxizeghqo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gppvknnbp.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhwniiuo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrpvciku.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/girviikmx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glgobvylv.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhfngusu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbrovhbtf.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsrabthn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/giglrezur.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gijffpbhg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gafaiaayc.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gijfvyvzv.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genhtaxvo.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gqctzomrn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/grkehqgmz.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/giqlbvfmo.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gugktgqty.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtsdczzc.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcrddurrr.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmytwzexh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gikednsad.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gvyycngkl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmvnuxggv.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdcfhvbe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghewqtzsy.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbsfzyiue.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gmgcaltrq.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhalanvy.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrqygwxr.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gjiotboyf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzphdjnjf.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtlylomkk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/geijdivns.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gdcuncxsg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gnqiaofhx.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gflsuonsk.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwhfjcel.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gqlibkcxd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzespcci.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gdxqrbnqz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gttmnusfz.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gmpbtqtqb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gpzivbvsh.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gypfbejhi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxqjemnu.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gzrtjvdlk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoehgzkf.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gppfrvywi.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqfuowdcj.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gvasnjqyb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gehbjmbcj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzsyteag.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gxdojxtce.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjdgyobf.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkzwqyrz.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpktrztt.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuglfbyt.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/ghzfeaugg.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkelxmsat.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggbrhheiu.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcltpdpn.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxohzfib.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrcunkbn.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqyrmaoc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxjwirqi.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gvwulhqud.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gykhrfawu.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcukzzbib.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giwclwljx.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttqfeivv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwxcakyw.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwqralikm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexcjuniq.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdweuqaia.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goyuyxfwd.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gssrohjbl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gfznyyjcv.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/ggewbsuuy.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwukztjho.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gtkdfikjj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gdrjesgtx.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfuazlygi.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gddsmpbit.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gfommihzh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gficaumwi.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gzawkhvyg.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/goyhnohqs.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gkukrqmfo.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gocoivojg.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpchoddua.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gdgilgfxs.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbfanypz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gfmpdqcpo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduitrfzu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlcinrsy.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzxerumz.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gdcudyswx.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvzqdxisk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ggnovxjqs.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gsejasqmc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshxeqakd.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzlhbbqn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrmgnaqk.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gvjcaybbi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gejgickdp.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkrzhkzx.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gwfhrqhgv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gjbuyxfft.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcdrgidt.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gufpjvoew.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbxigondj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfsjiawd.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gxchlasra.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgbavyrq.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfqirgms.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwtkljhl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/guwlgvccz.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjhepikz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbzxnqug.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaetnblfh.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gudjphhqd.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gjqurxlhw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvickwbv.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/guyrlacze.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gqrzodnov.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcruslkpq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gddsyesqd.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gspddjddv.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gbanjwyqu.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gexfrosbn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdryaxdt.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gggrxfmyb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuewrjcm.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrnnpkhj.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gomnuyzfm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdypsrkez.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmtnlhgh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaugvkhaa.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gntdympcs.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/geqpidqdy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvcxfbmsy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnuimpty.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoattbce.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gebrdccyg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/geldzohmw.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gqjgvrjbw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gaunxrthh.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gilmkggox.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfnwhcrhz.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmabkwejf.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gukkwjkov.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/giuzplirw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gqisdexnc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrhchlac.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnybdhuq.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/ghauoelba.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/glroxofoj.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gkzcjhenb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/ghwpomyaj.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glyclnxew.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gtvzvoazk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnxbvmkp.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gjhoeminx.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxxztlgj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/guylbyerj.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gevwxhuij.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gdjquwltm.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gymxjhuus.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzdjsoex.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfmhtamkl.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gypcimjqk.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gfdxifcqo.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqsggwyr.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsedumqy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gpwreaxxt.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkephfcep.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwabempqn.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gstytpwqx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gdoqdmzhx.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gqkzsaqrz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geivnwsjd.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/ghhtzihpz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gocoguaex.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gktmlkytu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhnssxne.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpogurowk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gslojkwfe.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gwydswdxs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gcedkfqtg.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gqseuxbny.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gwuzifwxb.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpeussml.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/glehdgjjb.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/ghfhkzlmb.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ggicdejvs.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpsffrrb.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyckswgkf.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmxzjhkq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfaluamy.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyubflit.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ghjhhmjix.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gohgjhdhg.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmyyfvre.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpcqirar.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/glvdpbqwi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgshsowa.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvsutsql.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvucddrbb.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gmajqdams.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gklnalplk.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gavragqzw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsufdkftn.sHtML


<!-- 参考信息 -->