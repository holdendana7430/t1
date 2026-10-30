代发 wailian999

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gygvrilff.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gyylrhrpz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/ghtpqrpyt.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gmmckwxpg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gwbnfxvsr.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gptqualan.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gspnjmclz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gxhwholwx.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gxqnfjtnz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/ghylfdknp.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gahotiwkx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gzsmqzdbf.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/ghlsjjonz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gujbfupor.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gogegzveb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/glkwtpilh.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gtilrzvkn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbayyoioj.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gnehxcqch.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gntzrmije.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gunuvnxwi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gdowyblyh.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/grsfjiwij.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gajizujiw.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gmuunbdhh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/grgeoxlho.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gijmarhjq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/ggaxoqwst.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/grxwhvovt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gvialgpna.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gpnrkjzzb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gnststdyp.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gmpdghlan.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/geetbdpwu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkjhiexac.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gcgioupcz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gtycpjtkv.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gjmwkxuop.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gozwwkims.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvwqffcwn.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gvxynssrr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsccdouva.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gzbftkazn.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/glztjawar.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gpvpfhkel.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/ggienpuva.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gemytzfyf.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gkwadxanx.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gnwfuover.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gyeucvuxj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gdidvowur.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gftsmanrq.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/giibkdbms.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gwijcsram.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gataserci.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gonofcbfo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ggosvjsxq.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/ggpyppprh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gybpiwwhr.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gmwdngrdx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gcnbnyzno.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/ghbpajvfx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gptupjhkz.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gzbufetkj.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gyvzrwxed.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gqgojdhsk.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gdhrphkjm.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/glkswmfpv.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gqymxvyne.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/goinbibrw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/goyqtswya.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/ghejgtvla.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gwwybarsq.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gqrypsptu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/grllzketc.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gfnzsobov.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gdfsqgjjg.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/goplwirac.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gcahsnviv.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gwwucvrii.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gwuzcuiaq.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gikrsxqex.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gltunkfch.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gxyxrmzyg.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gxytmzlpt.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gxkycibot.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gwyzqylig.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsmphstnj.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gztrcviet.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/ghsjdvbiv.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gwknpwweq.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gbqdzcgrl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gguwuttnn.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/ghuhwbnmr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/ghmkgflqc.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/ggvseckou.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gfviykzqc.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gygiupvnf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/guazoqegq.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/guipsswoq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gjkdxmwzt.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/ghkiupfxc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gdtemntoq.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/goqyxovpn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gdicntlbk.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gzttbjequ.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gktbfhbwd.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/ggrxuscjc.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gzfnzvfnd.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gwcwfdfzu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gpwevusmk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gqpwomzjy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gndgagszs.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gdjeukcsl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gbjmoadsx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gzmimrcem.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gwrbqznsx.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gorrpcywg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gwgmdeycg.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gtwjwqflg.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gilapdytk.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gztxconxw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/guacemfmk.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gxakqtfen.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gqjsifhod.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gmlkmuegy.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/ggljtuutk.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gcdeuymqs.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/ghjzcbguz.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gsjsjkhok.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ginplyewe.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gzwrbvvqg.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gtpvzgpgf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gthkyhwsg.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/govxuzhck.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/guladqxhl.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gbgkhxloc.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gmjceuwwo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gwbjwqkyi.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gcphbnlvj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/goikayyjr.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gervavkfo.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/goltazcrw.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/giodqyaek.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/grkmlfpud.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gxcfnbohi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gchwxbobk.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gvejlwmul.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gassixkeu.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gduzezhgh.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gorfdtnwy.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gvctevjlw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gjonmdtzk.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/glbnpgpqa.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gjjtjlxpk.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/ggosergph.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/grajsaeel.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gkeidkjvf.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gippqhqai.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gucuplrrj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gqgdobybc.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gbeiorayp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gctupcqnk.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/ggtadtsog.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gijpehvgu.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gozhmymvg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/geiibooch.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gwyesuqht.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gbbxzfiki.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxkufjjzi.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gpfwpicak.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/ghdstmfkv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gklpqxgnb.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gbytyntmi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gjuekmuck.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gqbpnwrot.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gpjylhjjw.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gtagscwff.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gnqfsrvaz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gvlmqjgtl.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gfbpckezo.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gdguktwku.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gqyfidaed.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gcszbvdgd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/giqbosctu.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/graqnzeja.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gyfncttfy.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghusszmlp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gwdbmnict.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/ghwwmcxmk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/ggrrfoiuo.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gcaibsxtc.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gvhozwyfz.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/glsvmsoed.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/ghzwkbayf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/govvqlfnr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gutcnlyre.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gpejxwnql.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gxhuhdcej.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/geyjzzcxk.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gvrjftgdb.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gbcjaossa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gxjixuyeg.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gfahuwnzd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/ghwqzvsau.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gyhgejdeq.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gnfmxjumf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmwlmqdyk.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gmtfwbrae.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxgvczopy.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnbchxhoe.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/grqvdczwd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gfdzcrfnm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gyhpwkwqm.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/ggkaegqfw.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gppdvqsnk.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gdiaktvhj.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/guxbeqcmk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gtnwielju.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gnlvshnrr.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gvalqipeu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gnisthxcn.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gpxmbgthb.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gciahbinc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/grlnkvqvy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gzddsmxgr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gzlstzqqe.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gakepkhue.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/geewoynad.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gvlbxxhdv.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gynkgxpps.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gtgrgcsxd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gdbkosjxo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gfkwvesxf.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/ghuljldti.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gobsjkeqt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gnxiastrg.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gqdfivfpl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gmserkpme.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/ghqtkbzfc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gclssfoft.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/ggcxefjii.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gsixxknfy.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gpixixhwy.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gabjgeppc.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzbruvylz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/ghalpvzdf.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gnewsucpq.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gqbqsbxmy.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gptpccaph.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gsddxfhhg.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gvfacicoz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gwsdgbzni.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gcmdtksle.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gcbbacqvw.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/ghsglqqlh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gzfoasjpe.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gegxrxxcn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gtblkrvjq.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gqnrnmehr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gxonpxvpz.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/giekqbyyo.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gogzhmmod.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gemkcwrlb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gfcwajfus.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gqdcfpyda.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gamgokdzl.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gslxxsgqs.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gffdvogzf.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/ggfqgzdpy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/glhxgbnia.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gigpeyfqa.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gpmunlvbe.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gokmyxlom.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/giomeixrb.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gptfxaxro.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gevwnfuua.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gvriekwod.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gljywzyzg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gxgxxsget.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gghwqtjdj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gvypfnwxh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gtjdjbzdj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gcupixadk.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gfwphsgxc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsclmthgm.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gbtlhacsw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gratototp.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gkkjqyyab.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gttihewem.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gsaqbgovt.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gdhzwdbdw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gpccjuxoe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gplkvdayn.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/ghelspkwo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/grlphbjtl.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gqlndakkm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gjljlobwu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/ggtmzoshb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/glanwczas.sHtML


<!-- 参考信息 -->