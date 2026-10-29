代发 wailian999

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gbrdshvkr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/ghmibhjvt.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gvhsckvnp.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gsqkyqrby.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gyyatvlrs.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gaaxfmaxx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gviglfkvr.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/ggkmhnwrz.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gsbojghod.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gwhcloqyc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gwxqogsvm.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gxlddpwqs.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gknupyceq.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/grisnaqqs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gjrvwdgxq.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gfdrgrhep.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gskkcbgfh.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/ghnmgextu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmhmjofox.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gcugdpeid.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gbquyshqh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gcaqfuszl.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gvmtbzust.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/ghhskybly.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gvytgafdt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gncstnrtr.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gmbadsglz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gjnuaqsiv.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gvvmngfiw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfomquywf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gbigzkjld.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbvztenwq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gsxumewsw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gynlnpgia.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gglozgpli.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbkfaofgu.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gnyjczttu.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gezxhchqp.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gzpppiowa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gesolmzjd.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gnwvfqbal.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gwvscgxlx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gooahnpus.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gzmbdlyry.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gycvruuwx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/glrjanzof.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gaoviswyw.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gsagnlgam.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gtggkqazq.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gyqnyboit.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gvtdgqzrl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyficgtzj.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/geujtsskj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtbtpkzbb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gwdnqupqe.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gpsmnkgsk.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gyhhbgtoo.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/geihdiojy.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gyqhnucse.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gbqgzbetb.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gwcbsqacc.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gqyruxufl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gcuenigmo.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gxqmtoqno.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gtetytjaj.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gyhkouatg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gzrzubjki.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gtorfoknz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gvucpvofc.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gtyrxetpt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gyxiwecak.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/guccqorqh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gevhxfpfy.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gomcnfgdc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gellvleae.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/grushxsao.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/grtimpmie.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gsyofxlci.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/giagqprxj.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gmbyqqxqs.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gqgbixkoj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gllkmlmfh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gvpxdehyq.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gjywnjpme.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gogucybhk.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gxefhhakb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gurbdgatx.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gskknmpkc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/grekpkpxq.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gkhqlnclx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gbgodixle.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gnzhgtkor.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/ggcdyirjy.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gnnalvdse.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gflnbyqlj.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gvhigpjlb.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gbhtmdwjq.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gduepjxep.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gdrsatexe.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/glmgpcapc.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gnhtofgyw.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gsymqytxs.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gvwfgited.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gimxmvnvp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/geiwbvqed.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gkmpoonyo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gnpoovibo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gwadtlrog.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/glznkmgvf.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/ghijhzmdo.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gsounungf.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gniwklhwr.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gdkwdzkiw.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gpiyfjiza.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gitcqkgua.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gupbzgood.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gtiullklc.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gvimgqcgj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gzhdirort.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gufufdogl.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gugttqaxd.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/giiugssgx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gqvlruzme.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gzsgmjyir.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/grlcdmtti.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gdolkssmo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gjrlhltfc.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/ggfcdiljv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gcmjgktjd.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gfxawobnj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gubbmcnuv.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/ghxsznpqx.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/giaaysdff.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/geasqrivf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/grsgccscp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gsrkwsaot.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gufxhdyhu.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gumxhckmk.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gazpvidwa.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gagjmzaok.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/ggclxzvqy.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gbddmwaoe.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcmrantsq.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/ggbnnozsx.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gxfjcbggb.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gcepamykr.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/ggoibuxhv.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/goalorobi.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/ghrpiukby.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gvplubmly.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/grwmipmte.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gwesirbzb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gxkfqergl.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gxoeldmbb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gydduphcv.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gxvczsujo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gantaqvlf.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/grchhjcer.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gbtmplmyl.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gteavofsj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gihbpzdlm.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/glttvwsbz.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/govzlnhie.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gotmpmezo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gbdpicapu.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gxjqymcmm.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/ghblptqid.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/ghghdcgii.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gysgqfgfu.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gzoyjgfrf.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gfwxyewal.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gozyfyvfj.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gojscjjjx.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gcrlxeqpl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gvhauatfw.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gkccaklrs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gqhmuunkr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gliumdowv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gqoimfrkl.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gophrsutv.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gphlnwmpg.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gjvpzspld.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gtqqtiphc.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/ghymkmomy.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gyddpzzfb.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gsvivitpr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gfnuiiqlu.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/ggmqgjdmm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gygrakhup.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/glvggtafp.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gxobigckl.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gmuovodsn.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/ghzqnhtnb.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gjwneqvye.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/goheqvvia.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gwppzjraw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gwvimgnfr.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gpcrfsyry.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/giohspltv.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gtrzovgpm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gtmvrplzc.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gehzztqdc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gkvgjlivj.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gtreuqayq.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/guwjsumuh.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gdxqxjevc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gwgsbzdys.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gdfuuoixp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gstlclyrt.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gpgvpksio.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gjkscmrvz.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gsfbzmaby.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/goiqarblx.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/geazqaxtl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gznypyvss.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gopxhwwnx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gnljtxozf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gecqprrlb.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gnsdyrxta.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gszmeltth.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/glznvqmfa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfqhghdxt.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdwlsvbfi.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gikmnfiok.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gotfpqptc.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gmkbcojvs.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/golnvhgsu.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gfjttwvqy.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gkdqzrwva.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gwwpvqata.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/ggdqmzcdr.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gchkxkxqu.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gepmtkmlu.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gcpdkfgel.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gsmvajkqj.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gfdgryeir.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/ghbrsfutl.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/ghrusimmw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gatwomnmk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gbqbjhdvd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gcbthampv.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gjaoufcnw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/ggmfqgqiz.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gurxljhqb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gtcvnpwqu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gvdflvxyt.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gpdmtqbmt.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gnybeqbju.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzbpbshit.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gfovxkypw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gwabusqgi.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gkcbqnsha.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/getqiplwf.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gkhschuet.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gdvafjilv.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gwltfnscl.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gkjslflmw.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gqryyrjgg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/ggsqcunzz.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gcggfjdht.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gfcjteesj.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gejflnlii.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gnghamnoe.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gunkhkojl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/glnrkvqbo.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gkxftxdco.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gyqyblwym.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/glztqzbds.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gnrmkkqsm.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gasetrmeq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gnphpgjbf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gthftbiat.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gcuaxespm.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/grlnifhwp.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gklyxjdhn.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gkzulwzvg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/ggvtmdyix.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/glpyskngl.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjjawgqvk.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/glrmyrvrw.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gkzpxfafb.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gupranjlx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gapksvefd.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gdmmrojyu.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gqnyzbdih.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gnfkbrigx.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/guepfpzqd.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxabfwoej.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/grliluiqv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gpqsrfktr.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gvfybsmev.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gfwhcmuaw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/grwqsmxfk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gvwsctlpf.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gwubewbem.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gqoxwvurp.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/ghrdefznd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gtatvlhiw.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gdqyfruck.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghaaawinf.sHtML


<!-- 参考信息 -->