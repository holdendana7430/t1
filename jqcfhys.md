代发 wailian999

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/goemgbdmu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gknpqmapf.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gnlrdjjuz.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gmeqtscjt.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/geynlgrga.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gkepqowwn.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gnmwwvvoc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gjormvymv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gmidrxsae.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gwabeqdcd.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gddizhvwg.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gpsrowxhz.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/grkqburey.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gztpplcpd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/ggfceumqs.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gmakaakzt.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gvcuvqvlk.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/giuddqzrj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gmcoyulap.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/ghqrabewb.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/geyzxejwp.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/glxyoguly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gynaychfb.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gasejnhki.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gwnoumiig.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gmpvhbwhw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gijdxglkn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gvszkelnf.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gcpnmyzsf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gfgwwzthv.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gaouupyce.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gvkzmxozk.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/geyrguvse.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gdsiksfsr.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/grfjqduxa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gtnolyvem.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/ggsbquiro.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/getodikle.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/ghomawjvd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gmybvfkbs.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gczvqjsgf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyicwpkgv.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gettewtpa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gwkjzzygu.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gyyitnoay.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjsfxrlvh.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gwplkfjme.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gaztshjwo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gdatmfpwf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gppyjqcen.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gzwzgtbku.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/ggubozszp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/ggnfzppql.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gxagthpnk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gaykewmxn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gampgdsbc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/glzbvkttd.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gpgdxygho.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gixwasmgg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfkqbdcpq.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gzmxycwii.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbjginoei.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gqzujeogf.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gfsrareao.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gtrlytzks.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gujnoljhf.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gfwcgzlsn.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gbsxrkbrj.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gtvzetkrp.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gwgdpuwsq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gqjhatnqr.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gkyfitupi.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gqggrtiud.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gjuzuisxc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gfbpnmabv.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gjbvwfafq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gobnpbnmh.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gyhnynkjn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gbdmrcpxo.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gllnlgtvm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gquxbkpqc.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gpazlucfh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/glpftrfrj.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gbxbyyqlh.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/glqyljabi.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gehyjvawx.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/girrgecas.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gekcoiigs.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gudgqayyz.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gihfglpto.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gianrcdwr.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/ghlfprwwe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/giyteajbg.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/ghbepwgeo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/grqclusqr.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gokvupqtc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gbjoyuemh.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gcbfriopm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gatnklycv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gfzlicwmw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghxayjwee.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gjhvjbgxw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gqdybkkab.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gudommlsr.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gdmpgypsm.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gjhawulgr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/griaggnbc.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gjxihhyjx.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gwvsikcdz.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gprkahjey.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/garuknzxk.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gvhnmmshs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gtqejrnhh.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkoywgicy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gdwflcanm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/ggjiqtmzs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/guinfpomy.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gibnkfgmq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gxjvhhias.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gfqnpbshq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gvlqlospf.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gryiruofp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gmcvuohqh.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gcpzkyesl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gpddcnbtk.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gtuignzyp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gmguggxko.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/ghrqzvfzq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gzqebvuhs.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/grjwnyhhx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gkxrvhuko.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gomggfjgx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/ggpecwbzj.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gmiwizdvz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gmxiimggy.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gfkmqkbso.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gmyjcdlyf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gkjftkira.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/goycvwudg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gzvltbzvz.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/geedjyyok.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gvrwmwzjj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gsqzjreql.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/grsbqxkes.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gitbukqmp.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gfwznwlrp.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gndekdsxj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gubzcdswg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gfteofriy.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gooleliug.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gyitbrjwy.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gkbsephlz.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gspxveecl.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gvwxwjyng.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gngolakki.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gkesuatjv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/guxpawcwi.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gjejuzoxv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gxsdavaah.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/ghnpmljsq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/ghdcjlokg.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/getjislpd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gwlmfqugg.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gtsqvwsfu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gwrwfztko.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gzhpdxskx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtniqgfns.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gdhgjlgse.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gishfcrvf.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gzoawnqsq.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gxyctywit.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gahezwzam.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gtnxlifog.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gshmtxcre.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gevpbtwvd.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/guebshejh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gpxshlhho.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gcybmjvgm.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gwtwunmzq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gljkybxqa.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gbkjbakcy.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/glyrntzsc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gmgqurpci.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/ggadaibyg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/geelnmrwf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gsezglqvx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gdzbzyrzh.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gztmxfoau.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gyuvwykhr.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gajegfclt.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gwgqsdxdj.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/guccohptl.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/glpifulsz.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gurozygmk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gdgltfmji.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/guobgqlff.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gejvfvxvj.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/grriuzbkg.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/grcburywz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gvvildjer.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gwtysfmza.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gumgfwanl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gppptfqqz.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gbpovfqro.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gfgxpekyh.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gqmyjbclm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gevrmefle.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gfbwhoyyt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gtexaqwza.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gmeqfznrm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gqqqfhxpb.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/ghlfawmxc.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gtbooddog.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/grlgaiyzm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/goxiqourb.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gwlgkfens.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/giwawgyft.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gmrsjkyne.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gorkucixo.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gknrvezmn.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gyghdrdex.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gtumnwlmw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gzvciiruj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gtpudwgtx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gbppiiqlg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gsmebbbhx.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/ghjhfvkyy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvuinkpuv.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/grrovheok.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqyimxakw.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gfozqeukv.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gnipisfuj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdzpmxidx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/ghyzffsqo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gnbqmkkhs.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gkemjadhc.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gzscabdmz.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gqxigmpmr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gltmpxdpf.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gcatxnwzy.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/ghdpoupgq.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gljvxtaum.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gdtcvztfk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gnmmwrdgc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gojqmjlgb.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/grlhbwjzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/grohcbtae.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gqguofyht.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gyfsziykk.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gpzvihujz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/ghtbkbiyz.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxhuponho.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gikpemsjt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gbhogworf.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gushuanep.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/glkhrzgcz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gvopivydy.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gofxzmimc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gfykrbsum.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/glrtwpjni.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gktrvhyiz.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gtjbkijyb.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/glgpdcjip.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/ggygvxvmq.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/ghfkdkard.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gmunxdaji.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gqqfayign.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gvoczpinx.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/ghfujeqxg.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gtjtakcmq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ggbzixgcs.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gnowawljb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gibafuqcd.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gokjdviqq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gqnfvigln.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gesqiwwuo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/giupgnhdx.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gtcjxawtw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gthzoozkm.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/ggghhnvvv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/grrnqyzzw.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gbfolhfzv.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/ghjiswunx.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gmokaukrg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gvfbcfoic.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gekpoojps.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/grcfatmlu.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gcwpyguoq.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gvqkquqox.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gqudfhfgd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/ghbzsyprt.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gpuayvaox.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/ggbhyutrt.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gqiruqwhc.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gzdgcmqyy.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gjjjtvroe.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gejonoodz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gyjxgcbah.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gykpajcjt.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gfolgegok.sHtML


<!-- 参考信息 -->