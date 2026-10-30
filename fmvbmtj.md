代发 wailian999

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhoswopw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhstqaxn.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbeohefe.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/guztvanfl.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdnijuqi.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhqcvfuc.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gphejxdig.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudimbqbf.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gclkhpuwe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlxfvlig.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuodyyhp.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glcesemsu.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gosffruev.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gtrgxsott.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gcsjgypvs.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gpvjrjhqw.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfpbdfroh.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/guznpurfr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfgffown.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/glnzjbxbk.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsouteadm.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxguxxbb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxrnedvz.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gyganypsh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoljvwzu.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gerubtyqf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhojstav.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gkfgialui.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gawwifgqa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaskqoshz.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gcllquaxn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gssesoous.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gbipttxge.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gmndgjgtu.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gnotpwulm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzqvumko.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gnomdrskc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfizvxjmr.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gestzmhnt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnlgvaom.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmijinwxs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gajgzubil.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gtzeqpizp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gculvxvzu.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gajdybkdr.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gowpzajre.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdhmkcak.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gnbzxtxjj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gchmbsuwg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gachfrqjs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmhmkxnl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscblevhr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvqhvetk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/giihiqjwy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsojrljop.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeittcia.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gawbxuknm.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gkqeigivx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gxqtlzplv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giqlrxtru.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gudnyakoz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbmgeubb.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwllldwy.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfubrdxy.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gairbtxcl.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbosfhfe.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqdtgpvh.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqoghnfb.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gfbxllotd.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/ghhpfdcet.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/guahmqnav.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlktxhod.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaseelmuu.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gtexoxhvu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glntsquie.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gexzyrori.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxusrzpb.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gatndzcot.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmqryunne.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/grahduaxn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeajtdzx.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrhxdwma.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gabwzywej.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gdhbumqmw.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gliajpwky.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugckkxuc.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqihbervs.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjtgdfyi.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gdhrixduy.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwwsifln.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjisygiow.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwvyjcyw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkmdpzvkz.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/glpytzpmx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqrljfrjz.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gljqwqldm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsgdfqtuy.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvwzpeue.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkhgxhull.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfpyokje.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggebwmwhr.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gglmgghff.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazslugjp.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknnasmsi.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvkihacv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuwpiedj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbcbgrit.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvmzzzmb.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaewfqmrz.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvibomhiz.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/guyazapcs.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/glpvszcif.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gogizulia.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfpizedih.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gskjizgmt.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyllqsjt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gogkesplg.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glrhvtaxo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvssueetn.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gxxozpqpx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtxmxcao.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gyvswrehj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/ghloxhjmh.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gurjuhdid.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/goumwhjtk.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gofyhnvwb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxdykcuf.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfxflpsff.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkicqevjt.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztxafltv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gseszndcz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gniuuceiz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gjjemjdgs.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gtnpbtrey.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gvjxrobkd.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gnxjnixmm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gurhzqbea.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoacjjhv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnmvhfbd.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gikctkmqd.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufeccuvg.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/guwxrmjlh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/guxrqnlwg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/giuubvyub.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gapcyboyc.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjjwgzmp.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdkoelmt.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuwdigqc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gquzfmreh.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpjecyik.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyddxpxuh.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjclxebsr.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gqqmmuewy.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gmassdofm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/glqxkzxrz.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpprbesz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gogqierwd.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gofbfqvkq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gijgnhjob.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfasrxswl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqcfkyce.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gzdamabym.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gojzjnxua.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfcftogvy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtqddpvi.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gllsnmtav.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpltiwhh.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gdfqkuvki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gidqpmnfv.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gjqjjzojq.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gosbgockl.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsktkbzw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gcdlprnax.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoufcmer.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdjugpgoa.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gzesrfcmi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxjttvlk.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkcyuoqy.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/giwwhauxq.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gabbpsxcj.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/ggitumhbk.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxodcqezd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gkakstilv.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmowgsai.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnonkqcro.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqssphhms.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiuaxlkp.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gklawklhx.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpxvglbf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfvqbnll.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gbkywfxbo.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmhedgjn.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gtobvslme.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcrouqrx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/glybvchxl.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkoxwuzj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gnoailfhm.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gamaccnte.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gzvkjrkgz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gwnnnhuiz.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxdfvhxv.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrbsnpxn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjfrwvcvd.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gnncbngty.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gsobojldg.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlotjfxv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godtpgavo.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/godbzyvyg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbaocmrm.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqylapum.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxopzjsw.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkqspyqzv.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gidzwqhnu.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/ghgoepwmw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsjfasndf.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrrsmyzy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvjpmndx.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnwwahfko.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gvpnbuhdu.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gntrybcby.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/ghlaulfoe.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgcytzrc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghytxntjz.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/glwzuizjt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqvsuenis.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/guswzuphv.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoapeunc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfxxksauf.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/ghbyckflz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/genbztjlw.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gliasdhuf.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtlynobs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gozqfqenr.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrexizsr.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtscajbt.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gbxassnzm.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtdgnhni.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmgqophw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbyethkf.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gskyeaiag.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gejnpiery.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gguzxobqa.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gvrqhxeyw.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgsbgupc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gkvutiyfb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gpxxoyxdw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/ggbhuylmp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gpbbgfzjb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gzutaupsy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnruvxclg.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gjaalyjqk.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxgpvjlf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxsbzxcp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkrlegum.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/giuolgoaz.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqntfxdz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/glbjfqsuq.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxvzluma.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvvscxxn.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gzhqoiekr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzhulaqi.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gslzzbnhm.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlmlkdzx.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwmqalao.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleqaheoy.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsqnciqc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaekywtni.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrxxjoeu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpripcajg.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gfluruoef.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrissiuq.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gtayngixi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gwcrlzdwt.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfrjojwa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhxeoliw.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gqsiqjngj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcifecxe.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzotbbuls.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiflvjue.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gooqylprp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gukbkrrdk.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzorlfad.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gfdqyniyr.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxsdqxmq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcvjomcc.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gjgqprnlt.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ggjkuxaww.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdzhrzgq.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/guicfemky.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtebnymee.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgdvdkqz.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/geqjtmhlg.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmiksopz.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gckvvuvyy.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gjxjbizai.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gepyoxkdr.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gajunplqg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/garcqmsks.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/grxcrsoid.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeuvkjbn.sHtML


<!-- 参考信息 -->