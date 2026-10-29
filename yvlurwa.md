代发 wailian999

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gcjzgfhjl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gdlpbbluc.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gfevkdcyb.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gxlsyqssv.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/grqcvtpgd.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/grpvhpqca.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/ghrbnufcl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gmuejbsap.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gwxlgdrxl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gnaphitbu.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gcsvepnnl.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gysuptxjb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gbjvzmwxo.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gubgjlnek.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/guvajnqqc.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gqvwdyybl.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/grxsdslhx.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gynccibfs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gidpfgigb.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gaxjrkacu.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gxuhxoswt.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/ghwoqnqxt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gsyzfhiqc.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gztlnaiyx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/guoegjujt.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gdnbcnyax.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdatmtbqp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gvapkycir.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gfhxdorta.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gaubnskae.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gsqspyzja.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfmtswm.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gkjwhfhiq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gardmmqqn.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/geskbqpqf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gbchnrrpd.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gdcpeexrm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gneuznspt.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gnlsyztrl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gexxvkjaq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gdpfkyocl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gslvmxhmn.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gmbcikxkr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gopjrdjtu.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gnhugkkab.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghqrtwhlm.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gvyujkgjs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gszrlybmt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gvhefkurs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gfnrwotji.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gcipbtnkb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gbhntqnhn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gdqfweafb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/ghfpfczlc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbdajonww.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gsgypatnv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gceetqefh.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gcrlbipuy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/guzwequjv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcjrnojgc.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/glhimvplz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtonokbuu.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gtaouatbr.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gvgzlbubi.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gvmfbqtqa.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gnojkhdly.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gzbdxnoza.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gjonkppvc.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gtntcxtol.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/ggdczmscg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gnzljngoy.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gzvrnlwma.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gdxmbybzt.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/ghjqcflzx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjzyatnq.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gxmksxskm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gwuxdrftf.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gjpjiximw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggjsxkadr.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gwgwfrhsf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gfgdislgs.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/glyzqlwaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gbzcsjjnu.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gvszgcrsg.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gkofztlfx.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gqwyvbqjt.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gytyccmqh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gweqmqqpa.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gqkavxzif.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gcelttktv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gvypsunni.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/glindcffp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gqqhlsibx.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gdmsdltpw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/grxpecywx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxjcualym.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gaxegmizk.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/geiaczxpi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gnbemsext.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gucpbzwsb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/ghhcqkgek.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gqvjyhrzb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gtmhejqht.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/ghyzgxgqx.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gzbfvphis.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gqgwklfko.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gvflajhvi.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/geqsgkojm.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gunfpapen.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gatjtslkd.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gadfigxii.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gfkajslnc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/goyyfqqds.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/ggqvwhyjf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gesrqcyhu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gqzpsjpko.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gkxhbovwi.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/ghjqsmwdr.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gbmkeakup.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gnnakkdyb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gumpnsnxv.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gmarlgncf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gpyieotwf.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gjjomabcw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gesexsmqx.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/ghgrthpcr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gmlktqnxi.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gdsqgwsqa.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gidnhpkys.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/grzvgzvte.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/grehoeody.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gxjzsacti.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gvlwatkmj.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gewgkkhuq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gxeaqsswu.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gnvyrroyz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gktcxbnbh.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gwefsrlyv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/goxadhyck.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/geceerhwx.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gxmulhcxk.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gqfbomlqm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/grgfbohzb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/ghwooeucc.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gbwtyyffx.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/giqpqjbqk.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gfxhbvezy.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gidrjztdw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gufkmlgqz.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gdfpzaaoi.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/guexpeygd.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/goaksfyjx.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/ggloxzirq.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/ghxwpblvc.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gmglzqfnr.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gbautvnkf.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/ggdltchtn.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gofspjgor.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gehciqphb.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gmzhzjrab.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxhaekgyo.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gxghmpmkz.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gflwjpila.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gwcuiudck.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gzqdibhpc.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gdejynapy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gvetgxigl.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/grmjuvcrs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gdhnyjvfm.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gndtkurje.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gatigyoqg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/guvhvfjzo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gggduxjeo.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gewvzyeki.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjuzgkdkm.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/goeqggsws.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gszrxclgn.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gylnzybxk.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gnicnhzog.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gckpdvppy.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gbgtvmlfu.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/glaegkwsn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gwouirmzv.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gqhxtfays.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gahjpjfru.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gqvgzalhv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gjycgxchd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gfforwicp.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gozebchwl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gqluotyaf.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/guwkyjtml.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gqlnvirep.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gbfqzgsug.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gijahcyhe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/glaszpyaa.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gzzbqmzfd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gijxrrraj.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gwhvvtodv.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gpqhqvwzj.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gehsobbcu.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gutwfixpa.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gsauguzns.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggzekrrod.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/guqpszbva.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gcwkmbyiz.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gshyjuhgg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gtnbnhlxq.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gppctxzqd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/glxhxilbj.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gmcwcooar.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gzasdhjzl.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gbenkzaxw.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gjyrbumeg.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gjqjftxse.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/guxbwbsft.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/grdzqwnxw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gllhafnuo.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gulboeyfo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gppswyrnq.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gspnkmubd.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gcsrlknjx.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/glnvqdgtx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gljuoqrnp.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gregxqntf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/ghwektees.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gmuvdruhl.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/grhnydpzh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goalvkxsr.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gpwwgulhq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdqonfzvu.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gomlmspja.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/grxknckfi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gfmbeikyg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gtigslsgr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gcjtbeimf.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gtxycztsr.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gsdpwldqt.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gbjgvcmkg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gcqbyznkt.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gfokwtlev.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gzmimnblt.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/ghhqdhvbn.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gvbelujjp.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gnskfkiug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gddlivyoy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/guzbklony.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/guhyptvyc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gwlqvwgfi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gghlvnbxd.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gzyavtgxk.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gvcdgjrjp.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gakzgpfqh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gijupznvq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gdrgnwlsc.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gmkzugyxp.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/glflfqeqa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gqftxzsfc.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/goqvbngmg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gajdbyuvt.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gdrihumby.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gnsjlrffh.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gjudxvvvo.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/glgddmglb.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gsuvsrbdn.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gcpmacpxq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gobumniih.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gqsjvbhxb.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gtyaxablk.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gddmvwoyd.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gweohoeao.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gdgannkeb.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gdilgkarn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gxwvvvptn.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gigqktmiw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gdafftkui.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gjlqrvqen.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gkrgurhtk.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gbgmusqzl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/ghqvavviw.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gyjbpqufz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gqyfclnet.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gwpwktawg.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gfgxozpux.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gnjcqezoq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gbzgzygic.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gurpbuzrb.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/goflbfddn.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gngqiktaz.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gbauoeemc.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/guixwuxcw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gpikhlcin.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gvezbyymx.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gmlbsfido.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gueowtlew.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gvnwgyles.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gvajaeyod.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gwdqiavnj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gcjnetzup.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gdymzutgb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gasipxiec.sHtML


<!-- 参考信息 -->