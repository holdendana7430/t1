代发 wailian999

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gynwlnyin.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gqxxmtzqe.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gemgszdxg.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gciuzluds.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gxxiykeva.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gpagkxfrz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gidttndvv.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gdgrxetqz.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gclzcpjbu.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/ghqqdlzip.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gxfhanibj.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gqzsbyvzg.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyknowomc.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gmirdpurb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gkdyehpfo.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gktxlegbo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gapsiipzu.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gfjpwgpnm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gyhxbgnwe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gbfuajebc.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gwhvryzrp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/guytjxlxc.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gwvgcbtvs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gzcircejg.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gaxqwiktq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gztlcrscf.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/ggopwjxpx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gbxkwtbeh.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gkvyoswhg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxeawsyne.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gtqvrcygx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsasehwfy.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gzuenwnzd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxqemupco.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gkzekyyyf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbpfyxrbp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gtppeflot.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gztzcusuy.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gyzbqkllj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gxinddcny.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gbmpvxuwc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gtpjikowk.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gfhxjlmqb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gboqcldjo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gufkeabxg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/glveasbfm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsuwyoqyi.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gtzzauxyl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gfoylfyjk.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/girclwdco.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gegslnsna.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gflbkxgok.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gewcxetyn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggusglvdb.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gdppilkbx.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gyxfeszdw.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/ghscbirrp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gbxjktbxn.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/giqikrjxp.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/glrnwvkpl.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/geoofilcw.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gxagomycw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gdtrnczpx.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gpolxckmy.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gwugplsmr.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gapioiyqc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gwmhbjmhp.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gzkldfrgs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gjfawxmpc.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/grfqnmlko.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gtmjmkvwy.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gtpuxikiv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gyymyqcnh.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gurjfjsmq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gvuhhrgmn.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gzsworzti.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gpswivuyz.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gdhwtzsnd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gpwdrwjco.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/grkugqaec.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gjlihhuiu.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gvplihgts.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gzksyxyqi.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gqwiwqvdo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/ggxmbwsce.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/geoqclgsj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/ghtpnfryw.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gpsrkgnwy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxgbqdcsh.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/grplemuim.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gtemkgiri.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gnhdwgdbb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gkoosiesb.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/glendnjoj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gudybhrua.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gfjqsxiau.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/glevngcen.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gwjswygby.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/grgbvqwuk.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gamzayocn.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/ggjmisjos.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gctobegep.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gmdmypyuw.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gozezpfcl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gvorgmbed.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gnuuxymfp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/ghpnxlxln.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/guysjepfi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gjpcnxdwt.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/giktdjgei.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gomynhdrw.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gbnvuqnbx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gblrlplko.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gnrkzepyq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gvtkyzqrq.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gdjjipnwx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gaokzowav.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gjnhwldlj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gxuetxybh.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gjfwmemqn.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gvjwsekks.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gpjrjzcwy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gafqvsyic.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gelbtzuqh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gwqwozuyx.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gfdyxxfkn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gaehokxgu.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gravanujf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gfydaxtht.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gbmtrzfsh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gykfhpfwi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/ggqsquhwp.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gvgozkcra.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/ggnuqxeqg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gbosbpleh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gdhnorthg.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gjymeyndq.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gzglbfxcf.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gilixagep.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gonnvjrhx.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/glrchkieq.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gxwnjahis.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/grtxuolsi.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gsagdnwwt.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gszvjrdqj.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gsljsfbqx.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gghgajgam.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gpzwzeogq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/grvphkjfk.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/geossztwt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gpuilyzrh.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gxzckpyxu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/geukyecov.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gxzhvprmy.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwmswzjmw.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gqfxppdgu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gozxompxx.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gvpbapbpk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/grsedjbip.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gmlzptcjs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gtpcpvzae.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gaqsnkfkc.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gjeatvvps.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gmdycpueb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gkkvflbzd.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gpvvkwesb.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/grcebwtnl.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/ghlhxtgbv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gblvqcuqs.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gwvfkwglh.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gbsbzamjd.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gzeykmcsg.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gpstzgrnp.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gxliihipm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gqsspittn.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/grcerztnd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gzizwyfxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gaxgrrnvn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gvessfany.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/garyivcha.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gfspwzpjl.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxxjxefdc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gtfdhycgs.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/geplnipqe.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/goizhossk.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gsonssnqx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gmyjqpfiu.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gwxblxeyp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/ggisoqsyi.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/ggyuthlna.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gsyneorrf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/ghwmmzfhh.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/ghuqemafc.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gmxvztccb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/goyjhntth.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gkyzhinjd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/geywvovka.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/goyjemiix.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gkrhvkcor.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gadpiyshf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gwjxuruxz.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gpliulckv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gnsfsonkr.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gqimfkhhg.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/ggxqqovlb.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gcjeoeazh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/goqtfcceh.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gafnbzflp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gotihgptn.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gvxudlbxy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/golvphtee.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gkxncwbot.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gqpesujqz.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gvmmyacec.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gqlzcelht.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gbmlaltrg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/glxxpbpag.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/ggxydcdhs.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gaoxcxzgu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsevpnckb.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gpacmwinh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzhrdeovf.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwwwmqoss.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gobohzzvx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/giufrlxjt.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gmypaudar.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gqpcfvusn.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gbgqvoigb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gjqfqbcqu.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gmrvzrciw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gpwtzbsvs.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gylvhfixl.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gupbgplxi.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gfpkxmdbk.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/ggsltymlk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gdtywiunp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/giwrwmsrf.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/ghfjjuwjm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gjcgoyduy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gbzgwjwyt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gwztiyorm.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gfbbxowbz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gmospkydg.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gbchbabjr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gzxxnamvu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gkjuvrpiw.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/ghjjkzgxy.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gijubjpsi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gzervacis.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gadypjrsn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gxktpqcjk.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gbthnobwj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gemnbyvuo.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gnfucubdp.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gananwwtj.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gznymdxca.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gebvjxrlu.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gwyfziczp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/glhlpnbtv.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gjzqgxhxr.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/ghxktqdxe.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gubxfyjkl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gaaowzmcp.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gethhjkwa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gqxggcoej.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gzvmguwmf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gxtgnfzje.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/goamzhweu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gzblgyled.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gygdbjzoy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gkbuzhzxe.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gcvxlvncc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gdrwcemlt.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/ggbavhjeo.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gmsouvvti.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gpmtvupzh.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/glovynhwh.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gifvzagvk.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gkbhwuusy.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gapskvtai.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gnsxzvogi.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gqngideln.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/ghdmqiibb.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/grgwahzbc.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gmmulvujq.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gbbexivua.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/ghggoedbk.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gqscygoam.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gusfqliwm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gqhmgtgcf.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/govdeuwyr.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gocpliowr.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gnlmtgjwx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gvuktzsuv.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gtbkmxpsd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/guaofebhg.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gevdxjyss.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ghwhkrueg.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/goshcnpfp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gxfzadatl.sHtML


<!-- 参考信息 -->