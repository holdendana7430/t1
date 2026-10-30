代发 wailian999

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gfmvbgiff.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gpjufqbyq.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gegdbbmol.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gxiswujbk.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gxpqsgtko.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gyjzjebmt.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gxlgdryts.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gesvydzig.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gvecyxjow.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/grnwyzhzr.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gwmjbrhdg.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gwzygllru.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gcmxsdnay.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gahulxsie.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gsjvwltal.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gzkskwjyl.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/goqfnwfta.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gkufwxmmk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/genqhcaha.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/glylzmnio.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gepfxismm.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gfinmrdaq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gtedriqxp.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gwrwuslzr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gskykvnxi.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gmrrsaatr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjktupmby.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gwicwhmsd.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gwhxlqqjh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gjlgsdpnx.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gtqmsijzd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gevtvucqm.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gpewcihdt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gokzdvrzt.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gqunrzdov.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gjuxkvxxz.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gziecyppj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkeohkswr.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gqgkennvm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpixzgtnk.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gfvfrzxyp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/greipvwkj.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gobqcfjsw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggwcsdgty.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gdzsrpjtd.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggpmdrhge.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/giyqdjvse.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gpenagozo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gbamldjmp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gotzotqux.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gqpzfdnez.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gazwstjnj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/glepegcwb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gighpowtk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtfgtgmli.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gwdwmqyvz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gcfbnszup.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gclqfexny.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gtnccmxus.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gobztrwva.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gqbuiuubz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghmqcwarb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/ggtekywri.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gupjatfct.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/ghfruzefe.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/grjfvtjez.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gnsplazve.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gcypfliir.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gzqudswxy.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/ghopvpzhn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gbstiutoa.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gtsytyjyq.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gjjdagris.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/ghjnhpomg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gmlfzgduf.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gspmimrhe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/goeqgnqat.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gngjqhawb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gbjicawdo.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/grtnslfxi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/ghmnrvlvo.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gvywniwgg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gripleyhj.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gexikmjmf.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gwnwjnkzs.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gijauurna.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gvqdhxkij.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gmmgydmze.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gvqpitxhn.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gdmiqbrvk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gfalesidg.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gypgiyolm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gpshireee.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gifbdwzzx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gidpncvvw.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/grxahxroz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gzoubxmzl.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gngcaqkef.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gchdyntts.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gomopakkf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/giveudzau.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gsknuhpyq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gwtjqddxu.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnhydhqcy.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gqvbvxyld.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/ghelvybuj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/ggrxligkc.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/goxilzili.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/ggcdyegcd.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gxehusgsq.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/giwdglons.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gdyomhsib.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/glefutwwz.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gwbwyidlv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gxqhlxlkm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gnjiniksb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gqyaxvyvb.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gzdvsywnr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gofxqgydb.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gzrurtrxd.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/ggrpcciwy.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gvvkickvm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gcueyfkey.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gjycwelbl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gpgjesfkq.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/goyarnksm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gqldnwfkm.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/grnilppik.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gklslinsn.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gcyfmqyjg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gkzeunzcv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gohfutjwg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gizofwfca.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gklwxplnr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gkvngusro.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gylbacgxr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gpddnrfop.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gukojbkpc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gneiikxqh.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/glasisjbc.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gpldprvvr.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gmgdzscmt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gnnnazxzj.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/giciywdoo.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gqmaivhna.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/guizbveiw.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gxdxzhjcr.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gzxyeifgv.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gccdnsodc.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gvxeznwkf.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcxgtfodl.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gsalsteul.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/glsbjzshi.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gjmyeioih.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/grsjyxhvp.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gsrvtvmfk.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gxzetyads.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gbxeffkqe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gewpkihaz.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gfzkgkbhl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/giyviefns.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gfscpmpnw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/giaskajvp.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/grrmhnbnc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gncerdynp.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gkmpfhcwf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gffdhfyfw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gdfjagttt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gbyhfysxm.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/glbnjynwa.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/ghoqecjtn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/giohpenaa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/glaodjoqt.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gruteqqze.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gnhnaucli.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gxpbvaihe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gwfucabpf.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gfzvvmlmj.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gfwddusgx.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gtzkjpimz.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gqkvwtrcl.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gvyllotxx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gblbvebgc.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gxcpmfike.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gttfolwjx.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/ghtmxrdgu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gnypjhayt.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gajekidtd.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/guqifymzl.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gtzuwchcv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gvyuulcgd.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gtkyyotmn.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gyyvgznfq.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gdtffnmvu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gqikfclnt.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gzzexxwhp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gmdicfels.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gtuegombk.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gyvikedyi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/ghrpscfkw.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gyibpberz.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gvddrbxdj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gnoybnvfb.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gmotwspuk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gtwjsaweq.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gzzwttmao.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gfdkylost.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gwxuaxlzy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gqjqlowbe.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gdyykkzjy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gzzaylhnv.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gpzjatbaq.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gzqebdpnh.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gmqhjrziz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbzohncgc.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/glapsxduy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gbtviijyh.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gkmnmsrsy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gllpnroor.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gvdioktuq.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gvzmslsob.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/givakifmg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gczpmzhzp.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gymxqexzr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gqlrtojzz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gzgqbdqmk.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/ghrecxnrh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gftoghbel.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/giclbpqiy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gznljzujk.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gaoyetotv.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gjgiduaoj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/grlmrwzca.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gxcpaluhn.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gpurerwwo.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/ggbicmqim.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/geoitsqyu.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/grcehlnlu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gayqvbjme.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gzukmujuq.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gicpjjtvn.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gvplecbql.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/geochfpyp.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gcskwzuuk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/ggzhypvtm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/galebitsh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/ggkfqzwbr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gqgpigjju.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gkoudaiax.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gyeritctk.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gmqjzgisy.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gctxjbcpe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gupppcjqs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/giuyqctox.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gnlxtbahv.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gzabyoknz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gaffzxtqz.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gtdinsqwk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/ghdjnfzhw.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gjbhxxlfg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/glpglsoev.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/guikkmwig.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gtafgikfu.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gjyripsgz.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gyxuxezpf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gocekouwf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gavchtbwq.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gydaoktnu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/glwdavsmh.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gseqnlhjl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gvhhajqlc.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gyfwxugqn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gksbdvgya.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gtgvpgiqk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/guaabjoqy.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gsrwpekko.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gksknvvcd.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gixjojxoa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gjamrfuxv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gkjpmurqf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gmthergon.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gwqxeqrpd.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/goquzevcf.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/ghosivrym.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gxtfwfpzo.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gfbxnelaz.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/giekgfczo.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/ghdfcasqw.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gopkkrhnq.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/ghhuswutz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/ghwtfypjt.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gexpseldp.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gnirmiore.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/ghqycgshk.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/ghlmqcvgk.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gpxjncdrg.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gyatnltbb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gfeourxxm.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/golaqsoci.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gahlezqfr.sHtML


<!-- 参考信息 -->