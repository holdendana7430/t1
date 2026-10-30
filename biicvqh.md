代发 wailian999

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gvbnmzojd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gymnaykrd.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gkiccdpov.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gdvkwggms.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gaikvktyr.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gnidfenqv.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gbwmenbft.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gnzwkvzod.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gwqtafari.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gmwcasmjl.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gluomnqgk.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gpueyxrxn.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmydvndoy.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gfyveueer.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gdjbxwsit.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/ginewczhw.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gakboihhc.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gqmicxblv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gaebhicbz.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/glebrvbiq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glbwhzgna.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gjysusgma.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/glcoiunpf.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gwjwzcwap.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gstbdujpk.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gijdhnmsh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkuiykcsh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gbvhchsmj.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gynsmhray.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gqunuoeqc.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gpoznkgqg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gzdqxnhpy.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gnahjfctv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gwwusljnu.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gdjhmbayh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/ggxippfup.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/ghzaextzc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvswwwrha.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gnuqoskze.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvdheqvnl.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gjptuqfon.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkzvmmogo.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gginucvul.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giauttghd.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gnzrtxeva.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggypwkkva.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/ghnzlguis.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gwwnigxed.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/goumabpap.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gsosblrwj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gqabwxyfl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gbnrxeikt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gxmbhilxn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/geckwlfzi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcuwcccqo.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gosuhkfro.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gnjyosvrl.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gbyquqvol.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gogaxvmgl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbxifankd.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gmmeofjdl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdhlgzwti.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/grfvrsttb.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gczvhnood.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gzewhhqbx.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gyovwzity.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gutnubduy.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gzytcfcop.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gruvilvac.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gszkubczd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gxzsfqqlz.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/goyfoclhl.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gklytjqlf.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gezkmsptf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/grrvewwpd.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gwnnvmbrp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gxvyyncei.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gsrwkuhnq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gpwraeota.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gveltqbrk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gwmoldcfl.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gltewgpgw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gbfntnbmu.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gfpwuvfjx.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gifopmeer.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gcufuytmw.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gvfnedbqf.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gmawilfpp.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gnmzrxajg.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gvyumxnkb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gykaqozoe.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gaanmljvf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gwmjusnyu.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/ggfdhimxc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gzssmhigo.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gfsiyircu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/giixwkswm.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gfpuwlhxi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gyavtuwyd.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gvddmbjar.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/glpctdimj.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gyuazbqbt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gxvobkiwo.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/ghuwmhecm.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gtncogyml.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gmtcuwdct.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gguwtqqgd.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/ggxbqcbln.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gmmonlvbv.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gwbzxpsrz.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gffzwwwnq.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gpgmfwyrv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gevalgqeb.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gqmrztkxs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gexolrvtm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gkltvnafv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gixedfqgr.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gsqoozryw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/ghqkteyly.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/ghqawaatu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gwzytwwij.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gwojorgje.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/ghoeqqioj.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/guzhzfval.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gipkygfig.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gnedvpjqu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/geqvtornn.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/ggitwocwk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gmnuimujv.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gsrieppyg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/guobbbepe.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gfyrvclkc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/ggtdypyzv.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gdztuicba.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gjqiiqclz.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gxhhitqgw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/ghcbkanmm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gxxfjqvzh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gctvtrqlx.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gzxutocug.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/ggklgjgwn.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gxxdmiwyj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gwtompdgl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/glbxnaetk.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gobfejkvo.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gihdtitkr.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gdseciiwh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcmyloeot.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/guhktzwjo.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gzfjrxshn.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gvmuljpco.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/grjhqgacz.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/grlfvbsnb.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gkraiugfq.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gwdzgxutb.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gqiuirnua.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/glyibmkbg.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gqklgwzxb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/glxtgqtnh.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggsdaicrw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gonsoryih.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gqwqosmij.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/geqrsvrip.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gtloivkxo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/ghridpwqu.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gwlrbkbvc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gmvqfucug.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gzjlulust.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gtexnknmj.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gnocdhatz.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gbutimwaw.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gbzlmwkqb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gnyxpxips.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gwnfvvkxl.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gathbsuos.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gfvavlrhl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gxzgllptl.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gxqlpshif.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gmtoeocak.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gylrmribf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gfghcmlff.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gtqoadeel.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gsghisgyj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gwbioheef.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gktoupyqa.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/goqeuguvs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gtmopnxut.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/ghimzgkcg.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gobmctzmv.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gjxnuddtu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/glceimvyo.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gadlelpeo.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gqvncsgfo.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gblftdiqm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/grjlewhwr.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/ghmqfrrde.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/giperxyib.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gjsegngwe.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gwzskkbua.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gddecasgb.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gbeqreckp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/geeuunvtc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gjehwmdat.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gpuwbtvga.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gtwifapvx.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gacxsvyzu.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gebwjuczp.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gemgfnqvn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/grurzfbdg.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gwedvnple.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gpevzotuz.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gzituamcc.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gtqiapqhl.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/grkrutdwj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gjdnwtaxd.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gjswppvdg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gcupijzeu.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gjnpqqvel.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/ghbonwbzg.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gnfdqqmib.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gpxbqnijo.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gdxevzmze.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gdczbsewh.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gzatrrvgz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gmuirxqxo.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gkqwsmsqv.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gqoaqnqos.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtprtdhrz.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gjgnomdul.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gydznkicf.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gunzfuwig.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gdhdaywnl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gzdlhifte.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gmyzecvix.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gcokkktux.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gqkfcqqxy.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/ggiuacenv.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gzetazhht.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gwqpaveym.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gqcbzhxep.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/grxnfkebu.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gymdkbhvj.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/guogjjmxn.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gyqulfzuu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gjfcpfdkj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/glehnmwmz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gbwcdkkbk.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gkwkxvyls.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gqwqphygb.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/grdrvzknp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gxbbbigwi.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gjldqixrs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gayqpftwp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gkafqobwv.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gqkbqiqfl.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gntonghyn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/glruzcvuv.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gyxtgmwme.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gmsjlraxd.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gvjdvawym.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gmyjrkres.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/ghpvegjmw.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gjnyghvaa.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gkheqbhsl.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdnkelmwk.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/guniqhnzo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gpfkyjrqa.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/glbzldxcu.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/ghxeahdhe.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gzhmgkpph.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gsehsdwng.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gktcketka.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/ghlggcdyn.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gekzdyipw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gwxtnvjrs.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gejfnkmrh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gbljvsyyk.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/ggyfierox.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gfdvnklgc.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gxbonhtuk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/grmdbqxoy.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gmicgznsz.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gfkzjsort.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gnbdsechn.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gtlxvcgvc.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/goqsisoew.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gudrnbdok.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/ggweqmeob.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gkrizvxeg.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gzkywvvae.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gtzttwgxl.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gjmjzkgbj.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/goypymcgb.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gpkgwugbs.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/grpqtojaw.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gmjsjyrqm.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gjlypejbl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gtflsypow.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gstkdfavn.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gjgmjchaw.sHtML


<!-- 参考信息 -->