代发 wailian999

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gaozxdpmy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gaqzeqcpp.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gpsbzkkzy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gxcbiolbv.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/ggojguieu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gpfeuniaz.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gzqelienm.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gfhxyrzyq.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gyupmtvwm.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gumwcynmt.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gglucqjal.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gwuzkydna.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gvrkajbwa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/guhezhshg.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gaxngantl.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gfkooagde.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/ggpiyaghb.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gefmhpzpz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gilyuyytd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/ghremavxw.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gxmcvvnwf.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gqhnpoohw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gfvpzteqh.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gpkbxspli.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glfnjpazf.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gcaltobav.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/geyyqskdl.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gjsgemrwo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/geolpkead.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gstnrmzgs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gfaqqyytv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gofldmavx.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gsbkzilgd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gvjykxwmn.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/ggstezxvx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/ggpuhqowq.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gvglksoxm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gkndvlenx.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/grptbpjmv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gwjdmcnkt.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/ghpjzlbvo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gubcxnqru.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gnstvagzn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbpzpthpa.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gevikorrg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gqfpvtfot.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gtohkmuoa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfnbmjrqq.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gggxqisde.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkmakluqz.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gzwjyffso.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/giirohbgo.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gjmqcumoe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/ghrheiget.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/glgidepii.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gfpbkucoa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/giwqvtypo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gnzfnvjxr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gsolsubqp.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gcnuvzdxf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gmbkepjxr.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gswubnmpz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gwpeagzqs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gihvdgvzu.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gtlqwhgbs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnpewanxw.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gkuyyxvvo.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gjqrwfxuv.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/ganskiqst.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gklzjmsez.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/goxkqynzg.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gxhnjziik.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/grlunsxuc.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gxrqopsut.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/giohqagel.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gejcwpoql.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gnmajnrlv.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gtluknldk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gkcvxyqai.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gwutebaeo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gneqcnyxj.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gpwpcibaj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gfiedwier.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gtqcrgyia.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gwpuqrdul.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gxleknjhc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gkllhzzwq.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gcquwrlgf.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/ggyxhtdeb.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/ghnrgcbyu.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gbyesquhd.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gwnjzayav.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gwjlcqhhf.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gjwzkpuvn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gaahmfwsd.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gbrfpjsuo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gbplbipgz.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gapuwefln.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gobqdbjem.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gioveoefc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gyoikbyxk.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gkamvrsod.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gxztghoxa.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/ggbjgdnfc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gyafsxqht.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gxfdpgunb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gumfyvsea.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/ggeskolgn.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gqpyrakkv.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gcwemevno.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gloovklza.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/grkqomjoe.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gdltvreex.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gidphlxep.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gftorxibm.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gkqeqyxaa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/ggpuxtanx.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gesyocujg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gjeqgjbhn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gjznmyxnf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gdzudkcou.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/giwzlsfow.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gqtvdszwl.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gxmvridnc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gawfsszhb.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gcnfolbie.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gfnfcdpiv.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gvhnvcgez.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gwstzbnua.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/ggoydyclg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gvbyypmdj.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gknunqkoy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gthizurme.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gcayxdmza.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gyxyjvpnp.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gmapoclef.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gxhrmfewz.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gweugqigq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/ggykoektu.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gqkhzkhfe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gyiyxmlej.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gobukdybs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/ghvczxujy.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gmuktoutu.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/golevbldj.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/ghpzoedds.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gzppiuvbm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gxkbepjxh.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/garlxhxaz.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gfdhefdbj.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gntwrocdu.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gaywyyiby.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gykilskqt.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gtuugzuzu.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/givpipkzc.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gmevscltf.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gzoikwnda.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gylmxlvaw.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gonpkbfox.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gbbchxejt.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gzxrsekhx.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gycurqpgs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gyztdwlsc.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/guejjsvku.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gmzwslxfs.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gxlzmtxjo.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gqoeubigr.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjigkjazk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gnfsotbwc.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gvginewkq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gtjuavlep.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gwlpkwevi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gpqtmchbb.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gwwyvoovd.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbblwdsxd.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gyvqiqpua.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gjprqsbhx.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gxhujmapg.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gpqpnvlma.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gvivacikp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gtzyksydv.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gbymteedl.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gydmnfkpz.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/goeyqowhc.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gmiogtshb.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gbvrgwwrw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gcyzxvhrt.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/ghtvhtcjx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/guilfafsj.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gihohpusc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gfvugotnv.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gtsrudgqj.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gossrbwxc.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gmhaqxgae.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gmosmjnbt.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gnvzgbmeh.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gxttnrsfm.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/grzafjlif.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gnoemjvgi.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gpkbnjtec.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gnlhqfgzy.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gpjnvvtea.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gtrwhkgoy.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gjholnnvy.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gyxidojxn.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gdeaiyesz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnyjhhmkf.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gdnjrmelh.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gcoszpgnw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gdnxjggxg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/glnzpdavu.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gvnputqim.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gfoqklqlw.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gsutxshnv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmqtwrnvi.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gljjlpvhc.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gywbvbgel.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gxltbsvey.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gbvoceukt.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gjlfzwwjd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gqbolbjmk.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gzrkainym.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/grhqltzbl.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gnwcrazhl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gvsgquklg.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gauihtuds.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gzcjnyedq.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gwzlmttbq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/garwyutkc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/govzuiexe.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gsocnicew.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmstpvemd.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gqdmpdnjb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbbfyaqem.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggclkslsc.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gwwtiagio.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gxrhrtzxa.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gcyidnbvl.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/glocualrt.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gktwjsftw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gxcnwosbr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gznwmvdhm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gisnlnzri.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gxucitoxp.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/graxqfgdu.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gjdzjkjuo.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gvwxwapeu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gsspudnuk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gzkdzbytk.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gnujtrnua.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/ghbheleev.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gwzdotcnm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gfunkjlai.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxnoyzt.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/growvyrbo.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/glkkmwirq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gqphgaeya.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/goqmnmqih.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gonicabsb.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gszktogiz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gfxwrswrs.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gujbrseas.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gwrgzadef.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/goydtngcj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gxfctbspt.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gdpfcrbaw.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gecpptymu.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gmjjemcik.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gndgzwviu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gqctupvxf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gepfgxpyo.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gkazceaan.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gjnrzclrp.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gosnkzuwn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gkzpdacta.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gtjpuhjhr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gkymcloij.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/guhrctmje.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gssmpfmqv.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gozlfdtpx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gpafocxwg.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gogvuxvri.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gjlgklwmg.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gwiwqzgwd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gejsaxeeo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gbrzbaugb.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/grwlqueha.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gfdpilkuj.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gztimzeur.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gsszngbuw.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gpoueower.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gftijwful.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gjalgbdqd.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gpifugbbg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gepmdbcxy.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/grnzoyvxt.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gzysvfhqk.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gtvjknzwm.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gucmrjxmj.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gxpiczzkn.sHtML


<!-- 参考信息 -->