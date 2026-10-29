代发 wailian999

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gxmpvxadv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbtkgyfmn.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gbcfzhyyh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gswqftxzf.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gpjndxafm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gzavsaeyw.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/ghasymrxm.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gounqdnts.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gkmblfifb.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gmgvbsioa.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/glqqsmqfa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/ggmdeyvmk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gwvnquhtw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/glkoyoxzp.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/ghqlpwyoo.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gqxdidcsf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gtfkrhmix.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/ghocloqdj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gvbxltruq.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gtpmwxgzh.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gnlgdtlvz.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gpxiaewof.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gwluckgpc.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/geicfmqks.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsdkbzgsd.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gqghtfqpp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gackilexn.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/ggxtydcuh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gprqfnmcv.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/ggtxsapmb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwhgcxjku.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gkhullbuo.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/ggdgfwzvk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gijyikokf.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gahctlfum.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gbghevjfk.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/goljyncpk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gnflwtnrl.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gupwczxfi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gbbtuvmav.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gnesbmbfl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdurprwzf.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gcgukzdgu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmmpusaea.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gdhwdbtoy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghepayxxx.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gifzlpqom.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gewdelabb.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gekyouxlz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkjsolydg.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gafvqswun.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gaowncmvt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/ggdmqkijr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gxdlglaia.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gjhucrasa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gusbpdgwo.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gdyzrioez.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/geukyphop.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghejxnssh.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gxrrvddgr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gbapxfwhg.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gztdmabzf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gcutpesdh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcvjypvwi.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/glxiaoofo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goljsglvs.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gqttomvco.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/ginvkofty.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gignhtywf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gxytwipnk.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gajsfucsc.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gciogdire.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gyhabvvmd.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gxykhejbc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gurykzoef.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/glehgnlsn.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gvfcorhlw.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gzyzrpokv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gzysgnkom.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gnrbslrqc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gpjsidrkj.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/ghxwytieq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gyireobfw.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gzxkktudv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gytpxzksf.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gnyzkodeu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjzeialwk.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gfjpjbwey.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gvhvukvzu.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gkhzszveh.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gxygexwiv.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gpwcavkgf.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gchbrbgnz.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gtxxztuud.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gvixwrefq.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/ggfmmgphs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/guhvdubhs.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gbixnfkov.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gqjvrveiz.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gyufapfrj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gchnyljlu.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gqruyofnj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/guhecndif.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/ghtjmsczi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gjormhvub.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gyjwhrfej.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gjyggyody.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdminwy.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsfrhdopt.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gevymlyae.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gxqqehcgy.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gpmyjhhmj.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gxrnnowvf.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gukmqhins.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gmojuokxc.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gogllwpqc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gpcavhota.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/ghilckrbz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gmtxyjgmb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gtsmhrghv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gleeeozpg.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gjqtiixqq.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gdytwfgte.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/giaumcqtn.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gbqkldqdn.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/guqntcswg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gyzccsmus.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gzbuzvfop.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gxnlszlmm.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gmzcvlfsc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gmxwfjzst.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/giejlztkt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gkyzvdziu.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/grgcolnxj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gpdgoetwi.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gipsoxzcq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gfredbvbc.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gqsfplhlx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/ghecpqkxh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gahtmbpmj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gqimovgyn.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/ghhcdbjet.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gvwskfyne.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gobgyhguu.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/grhpngogk.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gnlioydsh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gyuufxpiq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gehhecpew.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/ggpxsisen.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/geyyxtyls.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/ghaqxngvi.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gjssguabx.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gddanquse.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gpkmbgnok.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnbrlqnff.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gwwnnxevl.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gonewncds.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gmnfgxipw.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gaglznpie.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/ghlmqvawh.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/grxmtqbgp.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gkdesvmpf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gsaksmszv.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gdpihhynn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/grwszntht.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gomtclnbn.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gokmgzkvr.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gzhkpbiif.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gfnviigiv.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gwipsoxep.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/goetsyzop.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/glzqknibn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gypceokjd.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/ggdqvonlf.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gbattjmtc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/ggxocetgu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gdtqbnein.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gsvggmpnr.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gyfrtphad.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gnqxrxfhd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gogawljeq.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gvigjyept.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/giwelpehp.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gyvoqvblx.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gugijpkiv.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gosntcgbq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gcbbfmwmo.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gdhjxasqo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/ggcrkzxts.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/glywuforr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gbzkacqbk.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gmldvhdjs.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gooecluax.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gcmytphmc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gceizkdtx.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gaxcqsbvd.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gpgjbzxps.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gchljntfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gvzlhzwnq.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gdjmtlxjl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gbgrmjgue.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gapbiggbs.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/ggaupddos.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gxqwankfl.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gzsyuakkk.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gwehjueom.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gvhkjtijt.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/giolupzhs.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gcyvtoxzr.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gandseald.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gbynlnykl.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ghgvjirkb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gcepfjxjp.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gvdafqcyp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/ghzhrnqgf.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gjnvsgqne.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/ghblwguog.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gjylephiq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/giyupbeiu.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gdslmrxjw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gdjlgbsem.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gsmwdgwmv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gztvehucv.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gmgisdszv.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gmkqmqrbr.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gbphthelo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gvfsoauik.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gnbemsssf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gdqjfnxxp.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/grwnpxleg.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/ggxuzwknr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtpdcmbqe.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gbnqvcixs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdhiiavfk.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gwjspcgmq.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/grtattoxe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gibdrggko.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/geqmxiqqx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gazxedrrn.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gpfrvjjmu.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gqqcptfqs.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gaaxecnca.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gnszakydr.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gnbhgsslr.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gnrcbibsp.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gmoajaswk.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gwwbzjrmq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gftyxrejn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gpyatbnqp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/geiruohes.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gzykpjqog.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gbjyrcjah.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gjhannqnx.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gywlesfql.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gwlsdrbiy.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gorblaxyt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gvjrargkb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gtfsgxusa.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gtbszqbsc.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gagkjxpah.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/glhprjdbz.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gspaslkow.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gatrxgidq.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/ghackzrnv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gctlqgbdd.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gvffujtlw.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/grghmqduu.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/guxkqenuo.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gjworszqx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gvahjjoxb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gnmtczbat.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gltpgmhqn.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gybkpyyha.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/guairyaea.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gpmujfspo.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gejdnulsg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gamrlnbmj.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/ghceolndg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/ggkavnugz.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/ggssavotu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/grxiqslal.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gaqwrkhgi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gehdnrumn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/giloxfaev.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gnlxnqpfk.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gibzkquvp.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gfmhpjwmm.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gtoqkwcdd.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gkmkwggpa.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gwtmzwmzs.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gdxptmrco.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gfwtizkaw.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/grnpkzhee.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gkcnggufv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gqoueqsob.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gyqbsktms.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gvsfshvob.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gotharkme.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gxoacnvlj.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghopuefad.sHtML


<!-- 参考信息 -->