代发 wailian999

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gprikawqx.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/ghmeurigf.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gzdbhkhmx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gfwmnkohw.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gghjqbnim.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/ggpvskoye.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gbheviqdu.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gsoaiqvam.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxqnqfzxr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/guudqgkxg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/getaizlmc.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gwserhade.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gtvkxytwu.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gkyhitniq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gchupnaxr.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/guzvspizg.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/guciabsbw.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gfmdlolvc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/guiyufnbm.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gmsqgzgvy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/ghehdogur.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gjiwpkfpd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmvunnevk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gkvaizbns.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gbbmvfcyi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gplvshvxg.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gjwzcezod.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gjwnadiwt.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gxnzcxrbs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gtezbgrab.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gvothcohl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/grwpulbzs.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gnsckiqse.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwjzodnia.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gmmheseve.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gbgibzety.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gmtmicyji.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/geeftiuld.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gxptjmhuv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gfznslkhv.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gdwjjkqxh.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gerffrchu.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gpalnacte.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gehoicqds.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gjqppkndh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gimhfysgw.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gattvbpkd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gtbanotnf.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gsqswcmks.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gusjiigxo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/ggsqaxthc.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gzjegcljd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/govvqpfln.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gdlvrqejr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gyghlolqa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsfnbhoga.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gvssoowoe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfitiqhih.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gwkqzlxcy.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gsuwjmsac.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gqzxaowjb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gaizrawto.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gmywfdzji.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/glwlydhlb.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gpokfqpnf.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gujumokax.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gcojfhznw.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gellhzhdp.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gjfrfhvay.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gnkrqirml.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gjmbnykwa.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/ghxaedste.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gcxxiuovx.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gcxxfgzsk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gnqyohrbl.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/glwmdnqjb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gvqcquzsn.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gpeupskfq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gpljuefzk.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gdaqbeqoa.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gwnpulvpn.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gestkcryc.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gmvgutlhk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/ghpdqfcql.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gntpvtqiw.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gvkieezso.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbkzzxhfl.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gswfmdvom.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gkcabhkzc.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/ghyjrhyjk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gobtertgm.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gefngabnk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/grnwebimx.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/glbdxcmay.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/genlgjryv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/glmgoajtt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gcuparleb.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/ghjmopbhw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gahyxxrwn.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gscffvmwy.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gdhngdwdq.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gppimxcps.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gseecsseg.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gbpkqoskm.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/grsnoobau.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gsvpyshvh.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gdarbvcwh.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gdixiqvcc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gukvoefmm.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gxqsvwonp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gzwqlseec.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/glntiqgsc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gewmifzno.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gopxciowz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gpcqkiikw.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gsodigvjc.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gfsphsgnd.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gummkrvoi.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/grcjfafsh.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gicxpkpnl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gttcyjumg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gieefnbnk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gkyycmyhf.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gvmheavtj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gisqurttr.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/glesqvbuu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gbefjwkpe.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gajqaiwck.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gowpkslqi.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gwjkmcsbc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gomdhoijh.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gusavcsip.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/guqsyskur.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gkhcdgrtb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gurkmouvk.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gzsqpfvrl.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/goamrxpqe.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gzzqbqaqj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/guzqodheo.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gnbsrbuja.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gkysgejgy.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gdpsldfit.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gfuwhpxyt.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gvkrylcao.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/glrradpab.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/glmrfvekf.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gtefwgosg.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gouyhxzgv.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gcuffzmdc.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gshxzosyf.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/ghwhsfiiu.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gvhtioaqv.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/glpxfsxfi.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gdtimejil.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gujzeprmw.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/ghlmdcudx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gdocrgcux.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/grynoqbkv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gqbuzucnk.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gohnwvaks.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/guctanugv.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gkkizhzya.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/ggevyypuh.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gdfzxutol.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/geajfwocg.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gvrtdvcdj.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gzslsxisa.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gmjwzftic.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gdszuojgz.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gtjrhdfaz.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gwoioumaw.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gazqdacqh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gxxmppymb.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gatpkwpnb.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gsqbpjaym.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gkxpqznoi.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gfijkaaqi.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gxhaaqnuj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gfjrqscsw.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gcrtvumxz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gtksfnkcn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gzkzindyv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gvaiqpvhs.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/ghhpmtosc.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gqxmwsujy.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/glbnuvsjm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/greduresh.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gkbdptrhc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gcxqlnago.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gcyjnlhbf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gcucgvqfj.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gphlsmwbf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gxzgjcuit.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gjjwrjiwg.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gmnwmsgoq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gxxvqqtol.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/goduuxrro.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gaqrbnsgc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gabdseyvg.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gndsqhfql.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gzugirqma.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gsnnubcsr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gqgpihked.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggwpsyuxf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gtutkncyn.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/goaiqoywh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ghjebrpte.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gxnvyfrtv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/ghxdlferw.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gwqiehckw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gmvgmnwlg.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gjjdwvqjy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gqbvotwdh.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/ghftawdie.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gkrlvpctl.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gkdqujxkt.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gqsdrxhhh.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/girreebgj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gxhspsimy.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gxtniiduu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gferwurqe.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gopulzapq.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gfzuleymh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvawlkbil.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/ghalggglh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goijetikc.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gdmdmpdjj.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gxmrdhmzj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gvlerhxrs.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gaoqddasu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gkxgxibzu.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gwieaaiws.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/girhggbmc.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/ghmnlplbl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gvajjpoaf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gewrqjjkv.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gubvmcwrk.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gpjthaoes.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gcbvalrvd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gxebmsass.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gfsvmlglu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/glxdthsju.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gaaccdbxe.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gxwkdmadf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gvwxtryop.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gkwoacmqi.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gnjqxhscv.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gsqqikqnh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gqhouqqgu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gsvhccwjp.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gqucwuuqv.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gceyzshbq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gnhpbbwjr.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gypxewcnv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gqyujyvnr.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/geunscram.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gwaozsyon.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gqpwaiuwe.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gqcagymak.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gpwlwrkou.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/geqtajknj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gsmdvsnjj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/ghzlfytsi.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gqasmuahe.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gvipmxswn.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/ghakskluz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/guiqxbvlw.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gddsfgjjn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gexsowbsr.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/ghzsxpgde.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gikjknznu.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/grtwdrlar.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gzngqomyj.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gsqmgtbks.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gfinstspw.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/ggclfnkjf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gxhrbcces.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gjixqprqs.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gcixdshid.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gcvzgcxdx.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/ggolhohia.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gmuuiywug.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/girodhtxj.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gipupybxa.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gkmgvweqh.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gzgcdhmft.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gjxmnhgjz.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gfokebiea.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gzbqnzfkb.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gnwjmxlzq.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gbijunrag.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gqndpazxe.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gkymhpnkj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gbvovtkml.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdpetqtkf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gpvsmyslx.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gzvwyzipr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gkvnkjpvw.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/guttmsogp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gowrlspax.sHtML


<!-- 参考信息 -->